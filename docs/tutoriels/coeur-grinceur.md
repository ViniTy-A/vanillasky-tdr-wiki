# Tuto — Obtenir un Cœur de grinceur

Le **cœur de grinceur** (`creaking_heart`) ne se génère pas naturellement dans les dimensions voidées de TdR. Voici la procédure custom pour en faire pousser un.

!!! info "Vidéo à venir"
    Enregistrement vidéo à venir.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Cœur de grinceur — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
-->

## Pré-requis

- Localisation d'un **biome jardin pâle** (`/myseed` + chunkbase.net → Biome Finder, sélectionne « Pale Garden »)
- ≥4 **pousses de chêne pâle** (achetées au **marchand ambulant** trade tier 2)
- 1 **Œilchidée** (récupérable dans un jardin pâle, ou via marchand ambulant si proposé)
- Patience : la pousse a 10% de chance par essai

## Étape 1 — Préparer la zone dans un jardin pâle

1. Repère ton biome jardin pâle sur chunkbase
2. Construis un pont vers les coordonnées
3. Pose une **plateforme de terre** d'au moins 9×9 blocs dans le biome (les pousses de chêne pâle ont besoin d'au moins 4 blocs vides au-dessus pour grandir)

!!! warning "Biome détecté"
    La pousse doit grandir **dans** le biome jardin pâle. Si tu es trop proche d'un autre biome, le proc peut être moins fiable.

## Étape 2 — Planter l'Œilchidée

Plante l'Œilchidée au centre de ta plateforme.

L'Œilchidée se ferme le jour, s'ouvre la nuit — peu importe pour la mécanique, elle doit juste être présente dans un **rayon de 4 blocs** des pousses.

## Étape 3 — Planter 4 pousses de chêne pâle

Plante les **4 pousses dans un rayon de 4 blocs** autour de l'Œilchidée. Disposition recommandée :

```
. . P . .
. . . . .
P . O . P
. . . . .
. . P . .
```

*P = pousse de chêne pâle · O = Œilchidée*

Toutes les pousses doivent être :
- Sur de la terre / herbe / podzol
- Dans le biome jardin pâle
- À ≤4 blocs de l'Œilchidée

## Étape 4 — Attendre la pousse naturelle

Laisse les pousses grandir **naturellement** via random ticks (pas de poudre d'os).

Garde le chunk chargé (`/island keepalive on` si tu te déconnectes).

## Étape 5 — Le proc 10%

Quand l'une des 4 pousses grandit, elle a **10% de chance** de générer son arbre avec un **cœur de grinceur** intégré **au sommet du tronc**, à la place d'une bûche.

→ Si tu vois un bloc avec une **texture creaking_heart** (gros yeux jaunes) en haut du tronc, c'est gagné !

→ Sinon, casse l'arbre (récupère bûches + pousses), replante 4 pousses, réessaye.

En moyenne, **~10 essais** (40 pousses) avant de proc.

## Étape 6 — Récolter le cœur

Mine le cœur de grinceur avec une **pioche** (sans Toucher de soie nécessaire).

## Étape 7 — Activer le cœur ailleurs

Place le cœur où tu veux (par exemple chez toi près d'une zone de farm Grinceur), **adjacent à ≥2 bûches de chêne pâle**.

La nuit, le cœur invoquera un **Grinceur** (mob hostile qui ne bouge que si tu ne le regardes pas).

## Mécanique 100% renouvelable

Tu peux refaire la procédure autant de fois que tu veux pour avoir plusieurs cœurs. Chaque pose de 4 pousses + Œilchidée = ~10 essais avant un nouveau cœur.

## Astuces

- **Stock de pousses** : achète 20-30 pousses au marchand ambulant en plusieurs sessions pour avoir un buffer
- **Plusieurs Œilchidées** : tu peux faire **plusieurs zones de 4 pousses + 1 Œilchidée** en parallèle dans le même jardin pâle pour multiplier les essais
- **Bonus défense** : place tes cœurs dans une zone fermée pour confiner les Grinceurs à un endroit safe

## Liens connexes

- [Mécanique : Cœur de grinceur](../mecaniques/blocs.md#cur-de-grinceur)
- [Marchand ambulant — pousses tier 2](../mecaniques/mobs.md#fleurs-hautes-via-marchand-ambulant)
