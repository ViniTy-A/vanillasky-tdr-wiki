# Tuto — Ferme à mobs sans water stream

En skyblock, l'eau est rare au début (voir [Premier seau d'eau](premier-seau-eau.md)). Pourtant, la plupart des fermes à mobs vanilla utilisent un **water stream** pour pousser les mobs vers un killbox.

Voici les **alternatives sans water stream** pour construire des farms efficaces dès le early game.

!!! info "Vidéo à venir"
    Enregistrement vidéo à venir.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Ferme à mobs sans eau — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
-->

## Principe — Pourquoi remplacer l'eau ?

Une ferme à mobs classique a 4 composants :
1. **Spawn pad** : zone sombre où les mobs apparaissent
2. **Convoyeur** : pousse les mobs vers le killbox (souvent water stream)
3. **Killbox** : zone où les mobs meurent (chute, lave, dégâts)
4. **Collecteur** : hopper qui récupère les drops

→ **Si tu n'as pas d'eau**, remplace l'étape 2 par une autre méthode.

## Méthode 1 — Drop direct (la plus simple)

**Principe** : pas de convoyeur. Les mobs tombent directement de leur plateforme de spawn dans un puits → chute mortelle → drop collecté par hopper.

### Layout

```
              ┌────────────┐
              │ Spawn pad  │ ← light 0, plateforme solide
              │ (16x16)    │
              │            │
              └─────┬──────┘
                    │ trou central
                    │ (1x1 ou 2x2)
                    │
                    ▼
              ┌────────────┐
              │            │
              │   24+      │ ← hauteur de chute pour kill 1-shot
              │   blocs    │
              │            │
              │            │
              └────────────┘
              │  Hopper   │ ← collecte drops
              └─┬─────────┘
                ▼
              Coffre
```

### Hauteur de chute requise

| Cible | Hauteur min pour 1-shot |
|---|---|
| Zombie / Squelette / Creeper (20 PV) | 24 blocs (10 dégâts vanilla par bloc au-delà de 3) |
| Araignée (16 PV) | 22 blocs |
| Enderman (40 PV) | 44 blocs |
| Pour drop ½-cœur (player can finish) | 22 blocs |

→ **Standard recommandé** : 24 blocs pour éviter le crouching, et tu peux finir d'1 coup à mains nues.

### Comment forcer les mobs à tomber

C'est le **trick** sans water stream. Les mobs spawn aléatoirement sur la plateforme et il faut les inciter à tomber dans le trou.

#### Option A — Plateforme inclinée (trapdoors / slabs)

Place des **trappes ouvertes** ou **demi-dalles** en pente autour du trou. Les mobs marchent dessus → tombent.

#### Option B — Plateforme avec sand/gravel bias

Place du sable/gravier qui tombe au-dessus → quand tu casses le bloc de soutien, le sable tombe et pousse les mobs vers le trou. Utilisable mais one-shot.

#### Option C — Plateforme à un seul tile

Construis une plateforme **uniquement de 1×1 ou 2×2 tiles**, exactement au-dessus du trou. Les mobs spawn → tombent immédiatement.

Inconvénient : **très peu de spawns possibles** (les mobs ont besoin d'1 bloc d'espace), donc rate faible. À combiner avec plusieurs niveaux.

## Méthode 2 — Slime block + piston (push automatique)

**Principe** : un piston pousse un slime block sur lequel les mobs sont collés → les fait tomber.

### Setup

1. Plateforme avec mobs spawnant dessus
2. Piston collant connecté à une horloge redstone (~5s par cycle)
3. Le piston pousse un slime block qui balaye la plateforme et bumpe les mobs vers le trou

**Avantage** : push systématique, pas besoin d'attendre le hasard.
**Inconvénient** : besoin de **slime balls** (rare, drop de slimes en biome marais ou slime chunks).

## Méthode 3 — Hopper minecart sous la plateforme

**Principe** : tu **ne tues pas** les mobs via convoyeur. Tu **collectes leurs drops** automatiquement, et tu tues à la main / via lave dans le killbox.

### Setup

1. Plateforme de spawn avec trou central
2. Sous le trou : **rail + minecart à hopper** qui bouge constamment (loop de rails activés)
3. Le hopper minecart aspire les drops des mobs morts au-dessus
4. Le minecart passe au-dessus d'un **hopper fixe** → drops transférés dans coffre

**Avantage** : pas besoin de pusher les mobs, juste de les tuer et collecter.
**Inconvénient** : besoin de rails (besoin de fer + bâton — accessible une fois recette minerais maîtrisée).

## Méthode 4 — Lave kill direct (plus avancée)

**Principe** : au lieu de chute, **lave statique** dans le killbox. Les mobs marchent dedans, brûlent, drop des items cuits parfois (bœuf cuit, mouton cuit, etc.).

### Setup

1. Plateforme de spawn → trou central
2. Sous le trou : **bloc de lave** placé à 1 bloc au-dessus d'un sol solide
3. Les mobs tombent dedans, prennent feu, meurent
4. Les drops tombent (parfois cuits si la lave les touche assez longtemps)
5. Hopper en dessous collecte

**Avantage** : drops cuits (XP bonus, food utilisable directement).
**Inconvénient** : besoin de **lave** (donc déjà progressé jusqu'à pouvoir miner la lave d'un seau de lave Héros village).

## Méthode 5 — Soul sand bubble column (renouvelable, mais besoin d'eau quand même)

**Principe** : place une **soul sand** sous une colonne d'eau → bulles vers le haut qui poussent les mobs vers le haut. Tu peux ainsi les pousser à la verticale.

**Inconvénient** : tu as **quand même** besoin d'eau, donc pas vraiment « sans water stream » au sens strict. Mais 1 source d'eau suffit (pas de stream long).

→ Méthode hybride utile une fois que tu as 1 source d'eau.

## Cas spéciaux

### Ferme à creepers

Le creeper explose s'il te voit → mauvais pour chute simple. Solutions :
- Tue-le en chute 24+ blocs **avant** qu'il te voie
- Utilise un chat (les creepers fuient les chats — pas pratique en farm)
- Plateforme suffisamment grande pour que tu sois > 16 blocs des creepers

### Ferme à squelettes pour os/flèches

Plateforme + chute 24 blocs → drops d'os garantis. Combine avec un cycle « squelette tire sur creeper » pour disques (voir [Mécanique : Disques](../mecaniques/disques.md)).

### Ferme à zombies pour fer

Drop rare (3.5%), donc volume de farm important. Plateforme 16×16 avec drop 24 blocs, light 0 partout. Compte plusieurs heures pour les premiers lingots de fer.

## Astuces générales

- **Light level** : utilise un **luxmètre** (mod client) pour vérifier que ta plateforme est à light 0
- **Plafond** : les mobs ont besoin d'au moins 2 blocs verticaux pour spawner — ne fais pas de plafond trop bas
- **Distance joueur** : tu dois être à **≥24 blocs** du spawn pad pour que les mobs spawnent (mob simulation distance)
- **Mob cap** : MC limite le nombre de mobs hostiles à ~70 dans un radius autour du joueur. Construis ta zone d'AFK à exactement la bonne distance pour maximiser les spawns

## Combinaison optimale

Pour une **première ferme** sur TdR :
1. Plateforme 16×16, light 0
2. Drop 24 blocs au centre
3. Hopper minecart en bas
4. AFK à 24 blocs latéraux pour activer les spawns

→ Total ~50 blocs de stone + 7 lingots de fer (1 hopper) + quelques rails.

Pas besoin d'eau du tout pour ce setup.

## Liens connexes

- [Survie premiers jours](survie-premiers-jours.md)
- [Premier seau d'eau](premier-seau-eau.md)
- [Comment avoir de l'or](comment-avoir-or.md)
