# Tuto — Obtention de Shulker Box

En vanilla MC, les **shulkers** vivent uniquement dans les **End cities** du End extérieur. Sur TdR, le End est généré mais vidé → pas d'End city accessible. La solution custom : **re-respawn et re-tuer le Dragon de l'End**.

## La mécanique custom TdR

Mixin `EnderDragonFightShulkerMixin` : lorsque le Dragon de l'End est tué pour la **2e fois ou plus** , **un Shulker spawne automatiquement 4 blocs au-dessus du portail de sortie** (sommet du pilier de bedrock central).

```
Sommet pilier bedrock = portal location + 4 blocs vers le haut = position spawn shulker
```

Le shulker spawne **uniquement si l'espace est libre** (vérification de collision intégrée).

!!! info "Pourquoi pas dès le 1er kill ?"
    Le mixin vérifie `previouslyKilled == true` AVANT que le flag soit mis à jour pour ce kill. Donc :
    - 1er kill du dragon (flag = false → true) → **pas de shulker**
    - 2e kill et suivants (flag = true → true) → **shulker spawné**

Renouvelable à l'infini : à chaque re-respawn et re-kill, un nouveau shulker apparaît, de plus il est possible de dupliquer les shulkers ;).

## Pré-requis

- Avoir **tué le Dragon de l'End une 1ère fois** (donc avoir activé ton portail de l'End via les 12 yeux de l'Ender)
- Matériel pour fabriquer **4 cristaux de l'End** :
    - **28 verres** (7 par cristal)
    - **4 larmes de Ghast** (1 par cristal)
    - **4 perles de l'Ender** (1 par cristal)
- Équipement de combat pour battre le dragon une 2e fois (similaire au 1er combat)

## Étape 1 — Re-respawn le Dragon

Pose **4 cristaux de l'End** sur les **4 faces cardinales (N/S/E/O) du bedrock central** du portail de sortie (au centre de la fontaine de bedrock à Y=60).

**Recette d'un cristal de l'End** :
```
V V V
V L V
V G V
```

*V = verre · L = larme de Ghast · G = perle de l'Ender (vanilla utilise œil de l'Ender, mais on simplifie ici)*

Une fois les 4 cristaux placés, le dragon **respawn automatiquement**.

## Étape 2 — Tuer le dragon (2e fois)

Combat similaire au premier. Récompense XP réduite par rapport au 1er kill (vanilla).

## Étape 3 — Récupérer le shulker

**Au moment du kill**, le shulker spawne **4 blocs au-dessus du portail de sortie** (sommet du pilier de bedrock).

→ Monte sur le pilier de bedrock (ou approche en élytres si tu en as) pour tuer le shulker.

**Drop** : **1 carapace de shulker** (drop garanti à la mort par joueur, vanilla).

## Étape 4 — Crafter une shulker box

Une fois 2 carapaces accumulées (donc **2 cycles de re-respawn/re-kill**) :

Recette vanilla :
```
. C .
. B .
. C .
```

*C = carapace de shulker · B = coffre normal*

→ 1 shulker box.

## Cycle infini

| Cycle | Action | Résultat |
|---|---|---|
| 1 | Tue le dragon (1ère fois, vanilla) | Aucun shulker, juste les drops vanilla (œuf de dragon, XP massive) |
| 2 | 4 cristaux → respawn → re-tue | 1 shulker spawn → 1 carapace |
| 3 | 4 cristaux → respawn → re-tue | 1 shulker → 1 carapace |
| 4 | 4 cristaux → respawn → re-tue | 1 shulker → 1 carapace |
| ... | (répétable à l'infini) | ... |

**Coût par carapace** : 28 verre + 4 larmes + 4 perles + 1 dragon-fight = ~10-15 min de farming pour 1 carapace.

## Astuces

- **Capture du 1er shulker** : si tu veux **garder** ton premier shulker (pour la mécanique des élytres via Lévitation — voir [Obtention des Élytres](obtention-elytres.md)), ne le tue pas immédiatement. Encapsule-le avec des blocs.
- **Carapace puis shulker box** : pour obtenir 1 shulker box, il faut **2 carapaces** → donc **2 cycles** de re-respawn/re-kill. Compte ~30 min pour ta 1ère shulker box.
- **Larmes de Ghast** : drop des Ghasts dans le Nether (15-25% par kill, ou +Loot/Butin). Stock-toi en larmes avant de te lancer dans plusieurs cycles.
- **Stockage des cristaux** : les cristaux de l'End sont fragiles (1 dégât = explosion). Transporte-les un par un et place-les directement, ne les stack pas en inventaire mobile.

## Note de progression

Le 1er shulker = **chaîne fondamentale** :
1. → permet d'obtenir le 1er **élytre** (via Lévitation sur endermite)
2. → permet de farmer les **shulker boxes** en répétant le cycle
3. → permet d'obtenir un **inventaire portable mobile**, indispensable endgame

C'est l'étape qui débloque vraiment le **late-game** sur TdR.

## Liens connexes

- [Obtention des Élytres](obtention-elytres.md) — dépendance directe : besoin d'1 shulker pour faire un élytre
- [Mécanique : Shulker renouvelable (résumé)](../mecaniques/mobs.md#shulker-renouvelable)
- [Mécanique : Ender Dragon respawn](../mecaniques/mobs.md#ender-dragon-et-respawn)
