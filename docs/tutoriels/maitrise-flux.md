# Tuto — Maîtrise du flux (challenge Tier 3)

Succès Tier 3 qui débloque l'**Ornement des tourbillons** (smithing template `flow_armor_trim_smithing_template`).

Sur TdR, c'est la **seule** façon d'obtenir ce template — pas de drop dans les coffres-forts.

!!! info "Vidéo à venir"
    Enregistrement vidéo à venir.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Maîtrise du flux" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
-->

## Objectif

Tenir un **trident enchanté Impulsion** en main, avec l'effet **Pouvoir du conduit** actif sur toi, simultanément.

Le succès se débloque dès que les 2 conditions sont remplies en même temps — **1 tick suffit**.

## Pré-requis

- 1 **trident enchanté Impulsion**
- Un **conduit construit et activé** près de toi

## Étape 1 — Construire un conduit

### Matériaux

- **1 cœur de la mer** (voir [Mécanique : Cœur de la mer](../mecaniques/mobs.md#cur-de-la-mer-via-dauphin))
- **8 coquilles de nautile** (drop des nautiles, mob aquatique)
- **Cadre de prismarine immergé** (pour activer la pleine puissance — pas obligatoire mais recommandé)

### Recette du conduit

```
N N N
N H N
N N N
```

*N = coquille de nautile · H = cœur de la mer*

### Construire le cadre activateur

Pour activer la pleine puissance du conduit, place-le au centre d'un cadre de **prismarine, briques de prismarine, prismarine sombre ou lanterne marine** :

```
Vue de dessus, couche du milieu :
. P . . . P .
. . . . . . .
. . . . . . .
P . . C . . P
. . . . . . .
. . . . . . .
. P . . . P .
```

*P = prismarine (n'importe quelle variante) · C = conduit*

Plus précisément, le cadre est composé de **16 blocs de prismarine** disposés en croix autour du conduit, à 2 blocs de distance. Le cadre doit être **entièrement immergé** dans l'eau.

### Activer

Une fois le cadre construit et entièrement immergé :
- Le conduit s'ouvre (animation, particules)
- Il émet de la lumière niveau 15
- Donne **Pouvoir du conduit** à tous les joueurs dans un rayon de 32 blocs (jusqu'à 96 avec un cadre maximal de 42 blocs prismarine)

## Étape 2 — Obtenir l'effet Pouvoir du conduit

Reste dans le rayon d'action du conduit pendant que tu es dans l'**eau** ou la **pluie**. L'effet s'applique automatiquement.

Tu vois l'icône bleue avec une vague dans tes effets actifs.

## Étape 3 — Obtenir un trident Impulsion

Source : noyés à trident (drop ~8%) + enchantement Impulsion.

**Impulsion** (Riptide en EN) propulse le joueur quand le trident est lancé en pluie / eau.

L'enchantement s'obtient :
- **Table d'enchantement niveau 30** (RNG)
- **Livre Impulsion** combiné sur enclume

## Étape 4 — Tenir les 2 conditions ensemble

Place-toi dans la zone d'effet du conduit, en main droite ton trident Impulsion (pas besoin de le lancer, juste le tenir suffit).

Pouvoir du conduit + trident Impulsion en main = **succès `harnessing_the_flow` déclenché immédiatement**.

## Astuces

- **Combo Loyauté + Impulsion impossible** : Impulsion désactive Loyauté (le trident ne revient pas). Solution : utilise un trident vanilla séparé pour le combat à distance, et un Impulsion juste pour le succès.
- **Test rapide** : tu peux faire un mini-conduit (juste 1 conduit dans 2 blocs d'eau, sans cadre prismarine) — il donne le buff pendant 13 secondes seulement, mais c'est assez pour ton succès.
- **Combat** : Impulsion te propulse à 40+ blocs en un tir. Utile pour le déplacement sous la pluie, mais dangereux sous un toit (tu peux crash).

## Récompense

Le succès `harnessing_the_flow` se débloque, et tu reçois automatiquement **1 Ornement des tourbillons** (smithing template).

Utilise-le dans une table de forge avec ton armure préférée pour le pattern tourbillon.

## Liens connexes

- [Mécanique : Challenge Maîtrise du flux](../mecaniques/chambres-epreuves.md#maitrise-du-flux-harnessing-the-flow)
- [← Conquérant de la foudre (autre challenge)](conquerant-foudre.md)
- [Mécanique : Cœur de la mer](../mecaniques/mobs.md#cur-de-la-mer-via-dauphin)
