# Tuto — Obtention des Élytres

En vanilla MC, les **élytres** se trouvent uniquement dans les coffres des **End ships** des End cities. Sur TdR, le End est généré mais vidé, donc pas d'End city accessible. On a remplacé par une mécanique custom inspirée de **CarpetSkyAdditions**.

!!! info "Vidéo à venir"
    Tuto vidéo en cours.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Obtention des Élytres — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen></iframe>
-->

## La mécanique custom TdR

Loot table custom de l'**endermite** (`data/minecraft/loot_table/entities/endermite.json`) : drop **1 paire d'élytres garantie** si **les deux conditions** sont réunies à la mort :

1. **L'endermite est tuée par le joueur** (`killed_by_player`)
2. **L'endermite a simultanément les effets Chute lente ET Lévitation actifs sur elle**

⚠️ **Important** : les effets sont sur l'**endermite**, pas sur toi. Tu dois les **appliquer à l'endermite** avant de la tuer.

## Pré-requis

| Élément | Source |
|---|---|
| Endermite | Lancer des perles de l'Ender (5% chance par lancer en vanilla MC) |
| **Lévitation** | Projectile de **Shulker** (10s de Lévitation) → besoin d'1 shulker d'abord, voir [Obtention de Shulker Box](obtention-shulker-box.md) |
| **Chute lente** | Potion jetable de Chute lente (membrane de phantom + potion + poudre à canon) |
| Combat | Épée pour le coup final, armure recommandée |

## Étape 1 — Obtenir une endermite

Les endermites spawn quand tu **lances une perle de l'Ender** (~5% chance par lancer en vanilla MC).

→ Stock-toi en perles de l'Ender (via troc piglin ou tuer des Endermen quand tu en croises) et lance-les pour faire spawn une endermite.

Place-la dans une **petite cage en pierre** pour ne pas qu'elle fuie ou meure prématurément.

## Étape 2 — Obtenir un Shulker

C'est le **bloquant principal** : tu as besoin d'un shulker pour que ses projectiles appliquent Lévitation sur l'endermite.

Pas d'End city sur TdR → tu obtiens ton premier shulker via la mécanique de re-respawn du Dragon de l'End. Voir le [tuto Shulker Box](obtention-shulker-box.md).

→ Une fois ton 1er shulker en main, transporte-le près de ta cage d'endermite.

## Étape 3 — Préparer la potion jetable de Chute lente

Recette vanilla MC :

1. **Membrane de phantom** : tue un phantom (plutôt commun a partir de y64 après plusieurs jour sans dormir, ou drop occasionnel de cadeau de chat — voir [Mécanique : Pomme d'or enchantée](../mecaniques/mobs.md#pomme-dor-enchantee-via-chat))
2. **Potion étrange** (Awkward potion) : verrue du Nether + bouteille d'eau dans un alambic
3. **Potion de Chute lente** : ajoute une membrane de phantom à la potion brute
4. **Potion jetable** : ajoute une poudre à canon à la potion de Chute lente
5. **Potion jetable Persistante** : ajoute une poudre de redstone pour faire durer l'effet plus longtemps.

Total : 1 verrue + 1 membrane + 1 poudre à canon + 1 bouteille d'eau (+1 poudre de redstone pour la rendre persistante et la faire durée 4 min au lieu de 1m30).

## Étape 4 — La séquence de tuerie

1. Place l'**endermite** au centre de ta cage (ajoute y un plafond ca te facilitera surement la vie)
2. Laisse le **shulker** te voir → il tire un projectile → Tu t'alignes de façon a ce que le projetectile touche l'endermite et pas toi → l'endermite reçoit **Lévitation 10 secondes**
3. Pendant ces 10 secondes, **lance ta potion jetable de Chute lente sur elle** (tu peux aussi le faire avant comme celle-ci dure 4 min ca te laisse le temps)
4. L'endermite a maintenant **les 2 effets simultanément**
5. Tue-la **toi-même** (épée, à mains nues, peu importe — il faut juste que le dernier dégât vienne du joueur)
6. → Drop **1 paire d'élytres** ✨

## Astuces

- **Shulker captif** : capture ton shulker dans un cube fermé pour éviter qu'il téléporte (les shulkers TP de temps en temps sur les blocs solides)
- **Combo trident Canalisation** : une fois ton élytre obtenue, vise la combo trident Loyauté + Canalisation pour le combat aérien

## Note de progression

Cette procédure t'oblige à avoir déjà :
- Tué le Dragon de l'End une fois (premier voyage)
- Re-respawn et re-tué le Dragon pour avoir ton 1er shulker
- Stock de perles de l'Ender (Nether → troc piglin ou kill enderman)
- Potion membrane de phantom (phantoms en surface ou cadeaux de chat)

C'est donc clairement **endgame** (après avoir touché l'End et tué le dragon au moins 2 fois).

## Liens connexes

- [Obtention de Shulker Box](obtention-shulker-box.md) — pré-requis obligatoire
- [Mécanique : Élytres (résumé)](../mecaniques/mobs.md#elytres-via-endermite)
