# Tuto — Farm creeper-via-squelette (disques musicaux)

Tous les disques musicaux exclusifs (Pigstep, Otherside, 11, Creator, Creator Music Box, Precipice, fragments de disque 5) s'obtiennent quand un **squelette tue un creeper dans la BB d'une structure spécifique**.

Ce tuto montre comment construire un farm semi-automatique pour optimiser la rate.

!!! info "Vidéo à venir"
    Enregistrement vidéo à venir.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Farm creeper-via-squelette" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
-->

## Pré-requis

- Localisation de la **BB de la structure cible** (`/myseed` + chunkbase + Mini-HUD)
- Capacité de construire des **arènes de spawn** (~64+ blocs de stone/cobble)
- 1-2 squelettes (capturés ou farmables) ou un spawner squelette à proximité
- Compréhension des spawns mobs (light level, plateforme solide)

## Choix de la structure cible

| Disque visé | Structure | Position typique |
|---|---|---|
| Pigstep | Vestiges de bastion | Nether |
| Otherside | Fort (stronghold) | Overworld profond |
| 11 | Manoir (woodland mansion) | Overworld surface |
| Fragment de disque 5 | Ancienne cité | Overworld -50 |
| Creator / Music Box / Precipice | Chambres des épreuves | Overworld -10 à -30 |

## Architecture de l'arène

### Principe

1. **Une plateforme** au centre de la BB de la structure, avec un sol valide pour spawn de mobs hostiles (light level 0)
2. **Un spawn de squelettes** (spawner ou pool actif) sur un côté
3. **Un spawn de creepers** (pool actif) sur l'autre côté
4. Une **séparation** d'1 bloc pour forcer le squelette à tirer sur le creeper

### Layout

```
                         ┌──────────────────────┐
                         │  Toit (obsidienne)   │
                         │                      │
   ╔═══════════════╗     │   ╔══════════════╗   │
   ║ ZONE SQUELETTE║     │   ║ ZONE CREEPER ║   │
   ║   (spawning)  ║<─1──┤   ║  (spawning)  ║   │
   ╚═══════════════╝   trou ╚══════════════╝   │
                         │   pour flèches       │
                         │                      │
                         └──────────────────────┘
                              Tu observes ici
```

### Détails techniques

- **Toit en obsidienne** : pour empêcher les creepers de détruire la structure quand ils explosent
- **Light level 0 partout** : sinon les mobs ne spawnent pas
- **Hauteur de la zone** : ≥3 blocs pour squelette, ≥2 pour creeper
- **Distance entre les zones** : 5-8 blocs (le squelette tire de loin)
- **Sol** : herbe / pierre / pavé (peu importe, juste solide)

## Étape 1 — Identifier la BB

1. Active Mini-HUD côté client (voir [Setup client](../setup-client.md))
2. Type de structure → coche Stronghold, Bastion Remnant, Woodland Mansion, Trial Chambers, Ancient City selon ta cible
3. Vole / pont vers la BB indiquée par mini-HUD

## Étape 2 — Construire l'arène **dans** la BB

L'arène doit être **entièrement à l'intérieur de la BB** pour que les drops creeper soient affectés par la mécanique custom.

Construis selon l'architecture ci-dessus. Compte ~50 blocs de stone + 20 blocs d'obsidienne pour le toit.

## Étape 3 — Source de squelettes

### Option A — Spawner naturel

Si tu trouves un **spawner squelette** dans un donjon vanilla (zones de pierre, BB de structures), utilise-le directement. Ramène-le près de ta zone avec un piston-block-grace technique (avancé).

### Option B — Spawn pool

Plus simple : crée une zone sombre (light 0) au-dessus / à côté de ta plateforme. Les squelettes spawnent naturellement la nuit / en grotte.

## Étape 4 — Source de creepers

Crée une **zone de spawn séparée** (sombre, light 0) avec une plateforme accessible aux flèches du squelette mais pas aux explosions de creeper.

Astuce : les creepers ne spawnent que sur **sol opaque** (pas verre/dalles inversées) avec light 0.

## Étape 5 — Filtrer pour les kills via flèche

Le squelette doit avoir une **ligne de vue** sur le creeper pour le viser. Mais le creeper ne doit pas pouvoir s'approcher du squelette (sinon il explose).

Solution : **1 bloc de séparation** (par exemple une slabs basse), le creeper voit le squelette mais ne peut pas avancer.

## Étape 6 — Collecter les drops

Place une **hopper** sous la zone creeper qui mène vers un coffre.

Les drops s'accumulent dans le coffre. Ouvre régulièrement pour récupérer :
- Disques musicaux selon le pool de structure
- Poudre à canon
- Os, flèches (drops squelette)

## Probabilités attendues

D'après les pools de loot :

| Structure | Poids du disque | Chance par kill |
|---|---|---|
| Vestiges de bastion | Pigstep weight 3 | ~20% |
| Fort | Otherside weight 3 | ~20% |
| Manoir | 11 weight 3 | ~20% |
| Ancienne cité | Fragment 5 weight 18 | ~60% (besoin 9 fragments) |
| Chambres des épreuves | 3 disques x weight 3 | ~43% pour avoir 1 des 3 |

## Astuces

- **AFK farm** : `/island keepalive on` pour que ça continue offline
- **Plusieurs structures** : crée plusieurs arènes dans différentes BB pour collecter tous les disques en parallèle
- **Pour les fragments** : ne ferme pas l'arène ancienne cité avant d'avoir 9 fragments. Combine-les dans une table de craft pour obtenir le **disque 5** complet
- **Charged creeper bonus** : si la foudre touche un creeper dans ta zone, drop tête de squelette en plus

## Liens connexes

- [Mécanique : Disques musicaux](../mecaniques/disques.md)
- [Setup Mini-HUD](../setup-client.md#mini-hud-indispensable)
