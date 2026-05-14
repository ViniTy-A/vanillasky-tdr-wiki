# Tuto — Obtenir un Œuf de renifleur

Le **renifleur** (sniffer) est le seul moyen de générer du **sable suspect** et du **gravier suspect** dans les structures d'archéologie, donc indispensable pour collectionner les **tessons de poterie**.

Ce tuto montre la chaîne complète : œufs de tortue → noyé porteur → œuf de renifleur → éclosion.

!!! info "Vidéo à venir"
    Enregistrement vidéo à venir.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Œuf de renifleur — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
-->

## Pré-requis

- Localisation d'une **plage** (biome Plage — les tortues spawnent uniquement là, sur le sable)
- 2-3 **herbes aquatiques** (pour la reproduction des tortues)
- 1 **lit** près des œufs de tortue (pour skip les nuits sans les casser)
- Patience : taux de spawn ~1% de noyés porteurs

## Étape 1 — Trouver et reproduire des tortues

### Spawn naturel

Les tortues spawnent **uniquement dans le biome Plage** (sur le sable des plages classiques). Vole/explore le long des côtes de ton Overworld pour en trouver.

### Reproduction

1. Capture 2 tortues (laisse, ou pousse-les avec des blocs)
2. Amène-les sur le **sable d'une plage** (elles ont besoin de sable pour pondre)
3. Donne à chacune une **herbe aquatique** (pas de l'algue !) → mode amour
4. Elles se reproduisent → une tortue **enceinte** retourne sur la plage où elle est née
5. Elle creuse, pond **1-4 œufs de tortue** sur le sable

!!! warning "Herbe aquatique ≠ Algue"
    Sur fr.minecraft.wiki vanilla, **algue = kelp** et **herbe aquatique = seagrass**. Les tortues mangent les herbes aquatiques (seagrass), pas les algues.

## Étape 2 — Protéger les œufs de tortue

Les zombies/noyés **détruisent les œufs de tortue par piétinement** (vanilla).

Mais sur TdR, le mixin `TurtleEggBlockMixin` **annule cette destruction pour les noyés porteurs d'œuf de renifleur**. Les œufs survivent au piétinement de ces noyés spécifiques.

**Donc** : laisse les œufs accessibles aux noyés, mais protège-les des autres mobs (zombies, husk) avec des barrières.

## Étape 3 — Attendre un noyé porteur

Sur TdR, **1% des noyés** qui spawnent ont un **œuf de renifleur dans leur main secondaire** (visible quand tu les approches : petit œuf vert tacheté tenu à gauche du corps).

### Setup AFK

1. Place tes œufs de tortue près d'un océan / rivière
2. Crée une zone de spawn de noyés (sombre, proche de l'eau)
3. `/island keepalive on`
4. Attends quelques jours en jeu

### Identification du porteur

Inspecte visuellement les noyés qui spawnent. **Œuf vert tacheté** dans la main secondaire = porteur.

!!! danger "Drop chance = 0"
    **Tuer un noyé porteur ne te donne JAMAIS l'œuf**. Le drop chance de l'item dans la main secondaire est mis à 0. Tu **dois** le laisser planter l'œuf via les œufs de tortue.

## Étape 4 — Laisser le noyé casser un œuf de tortue

L'IA du noyé / zombie inclut un objectif **`RemoveBlockGoal`** qui leur fait casser les œufs de tortue (vanilla normal).

Quand un noyé **porteur** active cet objectif sur un de tes œufs et finit l'animation de destruction :
- L'œuf de tortue détruit → **bloc d'œuf de renifleur** apparaît à la place
- La main secondaire du noyé est consommée
- Un message peut apparaître si tu es proche

## Étape 5 — Récolter le bloc d'œuf de renifleur

Mine le bloc avec **n'importe quel outil** (pioche, pelle, hache, ou main nue) — drop garanti, pas besoin de Toucher de soie.

## Étape 6 — Faire éclore

Place le bloc d'œuf de renifleur où tu veux. Pour **accélérer l'éclosion** :

| Support sous l'œuf | Temps d'éclosion |
|---|---|
| **Bloc de mousse** | ~20 min |
| Autre bloc (terre, herbe, pierre) | ~5 h |

!!! tip "Bloc de mousse"
    Sur TdR, le bloc de mousse s'obtient via le marchand ambulant (trade tier 1) ou via l'évolution de bloc de mousse pelée. Worth it pour l'accélération x15.

## Étape 7 — Le renifleur creuse pour les tessons

Une fois adulte, le renifleur creusera des trous dans le **sable** ou le **gravier** qu'il croise.

### Mécanique custom TdR

**Quand il fouille à l'intérieur d'une structure d'archéologie** (pyramide du désert, ruines océaniques chaudes/froides, ruines du sentier), il y a **10% de chance par fouille** de convertir le bloc sable/gravier en **sable suspect** ou **gravier suspect** avec la table de butin de la structure.

Brosse ensuite avec un **pinceau** pour récupérer les tessons.

Voir [Mécanique : Œuf de renifleur — étape 5](../mecaniques/mobs.md#etape-5-sable-suspect-via-renifleur) pour le détail.

## Astuces

- **Plusieurs porteurs** : tu peux laisser le farm tourner longtemps pour collecter plusieurs œufs (un renifleur produit déjà beaucoup de suspect blocks sur sa vie, mais 2-3 renifleurs c'est mieux)
- **Sécurise tes renifleurs** : ils sont passifs et peuvent mourir en chute. Garde-les dans une zone close
- **Combinaison** : couple ce farm avec le farm de tessons via coffres-forts uniques (tourbillon/rafaleur/hache) pour les 23 tessons vanilla complets

## Liens connexes

- [Mécanique : Œuf de renifleur (chaîne complète)](../mecaniques/mobs.md#uf-de-renifleur-chaine-complete)
