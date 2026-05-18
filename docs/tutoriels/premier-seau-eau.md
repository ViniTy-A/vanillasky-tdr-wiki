# Tuto — Comment avoir de l'eau

Sur ton île, pas de lac, pas de rivière, pas d'océan. Voici la **vraie** procédure pour avoir ton premier seau d'eau sur TdR.

## Étape 1 — Réunir 7 lingots de fer (pour le chaudron)

**La seule source de fer en early game** : tuer des **zombies** par **player kill**.

### Drop rates réels (vanilla 1.21.11)

Le zombie a une **chance de 2.5%** de roller son pool "rare drops", qui contient 3 items équiprobables (fer / carotte / patate). Donc pour le **fer spécifiquement** :

| Looting (Butin) | Fer / kill |
|---|---|
| Sans | **~0.83%** (≈ 1 fer / 120 kills) |
| I | ~1.17% (≈ 1 fer / 85 kills) |
| II | ~1.50% (≈ 1 fer / 67 kills) |
| III | **~1.83%** (≈ 1 fer / 55 kills) |

→ Construis une **tour à mobs pathfind** qui ne nécessite pas d'eau (voir [Ferme à mobs sans eau](ferme-mobs-sans-eau.md)) et farme les zombies jusqu'à avoir **7 lingots de fer**. Sans Looting, c'est ~840 kills en moyenne (avec variance énorme). **C'est très long** — c'est la phase la plus pénible du early game.

## Étape 2 — Crafter le chaudron + le poser

Recette :
```
F . F
F . F
F F F
```
*F = lingot de fer · 7 lingots au total*

Pose le chaudron **dans une zone exposée au ciel** (pas sous un toit). Sans accès direct au ciel, la pluie ne le remplit pas.

## Étape 3 — Attendre la pluie (long)

À chaque tick de pluie, le chaudron se remplit légèrement. Compte plusieurs **dizaines de minutes** de pluie effective pour avoir un chaudron plein (3 niveaux d'eau).

La pluie elle-même est aléatoire en MC (12 000 à 180 000 ticks entre deux orages = 10 min à 2.5h).

**→ Patience.** Profite de ce temps pour farmer plus de fer (voir Étape 4).

## Étape 4 — En parallèle : 3 lingots de fer supplémentaires (pour le seau)

Pendant que le chaudron se remplit, continue de farmer le zombie spawn pour avoir 3 lingots de fer en plus.

Crafte un **seau** :
```
F . F
. F .
```
*3 lingots de fer*

## Étape 5 — Récupérer l'eau du chaudron

Quand le chaudron est plein, clic-droit avec le **seau vide** → seau d'eau. 🎉

## Étape 6 — Une fois ta première source d'eau obtenue : eau infinie via fioles

C'est le **trick essentiel** pour ne plus jamais manquer d'eau.

### Procédure

1. **Pose ta source d'eau** : clic-droit au sol avec ton seau d'eau (entoure-la de blocs pour éviter qu'elle s'écoule partout)
2. **Remplis une fiole** : clic-droit sur la source d'eau avec une **fiole vide** (glass bottle) → tu obtiens une **fiole d'eau**
3. **Vide la fiole dans un chaudron** : clic-droit sur un chaudron avec la fiole d'eau → ajoute 1 niveau d'eau au chaudron
4. **Répète encore 2 fois** (étapes 2-3) : au total 3 fioles d'eau = chaudron plein
5. **Récupère avec un seau vide** : clic-droit sur le chaudron plein avec un seau vide → seau d'eau

### Pourquoi c'est infini

- Une **source d'eau** ne peut **pas** être vidée par des fioles (seule l'extraction au seau la vide)
- Donc 1 source d'eau = nombre **illimité** de remplissages de fioles
- Et 3 fioles = 1 chaudron plein = 1 seau d'eau récupérable

**Conséquence pratique** : avec 1 source d'eau initiale + quelques fioles, tu peux remplir autant de seaux d'eau que tu veux sans jamais consommer ta source.

## Récap visuel

```
Phase 1 (long) : ~1200 kills zombie (à mains nues / épée sans Looting) → 10 lingots fer → 1 chaudron + 1 seau
Phase 2 (long) : Pluie → chaudron plein → 1 seau d'eau ★ première source
Phase 3 (∞)   : 1 source d'eau + fioles → infinie seaux d'eau
```

## Astuces

- **Plusieurs chaudrons** : si tu peux te permettre les lingots, plusieurs chaudrons en parallèle = remplissage en parallèle pendant un orage
- **Source infinie classique** : une fois 2 sources d'eau placées à 1 bloc d'écart, le bloc central devient une nouvelle source = source infinie de l'autre côté

## Liens connexes

- [Mécanique : Recettes minerais](../recettes/minerais.md) — utile **après** avoir du fer en stock
- [Mécanique : Seau de lave via Héros du village](../mecaniques/mobs.md#seau-de-lave-via-heros-du-village) — pas pour l'eau, mais procédure similaire pour la lave
