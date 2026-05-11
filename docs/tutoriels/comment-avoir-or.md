# Tuto — Comment avoir de l'or en early game

L'or est essentiel en early game pour fabriquer des **pommes dorées**, indispensables pour **soigner des villageois zombies** (et donc débloquer le trade émeraudes → marchand ambulant).

**Objectif typique** : 16 lingots d'or = 2 pommes dorées = 2 cures de villageois zombies.

!!! info "Vidéo à venir"
    Tuto vidéo en cours.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Comment avoir de l'or — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen></iframe>
-->

## ⚡ La méthode principale : ferme à cochons + paratonnerre

### Le principe

1. Construis un **enclos de cochons** avec **beaucoup** de cochons dedans
2. Place un **paratonnerre pas trop haut** dans/près de l'enclos
3. Attends un orage → la foudre tape le paratonnerre
4. **Les cochons à proximité du point d'impact se transforment en piglins zombifiés**
5. Tue les piglins zombifiés → drop **pépites d'or** (et parfois rare **lingot d'or**)

### Pourquoi ça marche

En vanilla MC, un éclair qui frappe à moins de **~4 blocs d'un cochon** le transforme en **piglin zombifié**. Le paratonnerre **attire** la foudre pendant les orages dans un rayon de 32×4×32 blocs.

→ Tu canalises la foudre vers ton enclos via le paratonnerre, et **tout le bétail dans la zone d'effet se zombifie d'un coup**.

### Pré-requis

- **1er cochon** : pas trivial à obtenir (pas de spawn naturel dans l'overworld voidé). Options :
    - Baby zombie monté sur un cochon (très rare spawn) → capture le cochon
    - Plateforme d'herbe dans la BB d'un biome plaine/savane → spawns naturels possibles
- **Carottes / pommes de terre** pour reproduire (drop zombie via player kill — voir succès `zombie_crop`)
- **1 lingot de cuivre** pour le paratonnerre

### Étape 1 — Obtenir le premier cochon

Selon la chance et ta progression :

| Méthode | Difficulté |
|---|---|
| Baby zombie qui spawn monté sur cochon | RNG, rare |
| Plateforme d'herbe dans BB plaine → spawn naturel | Si tu peux atteindre la BB |
| Trade marchand ambulant (parfois œuf de cochon) | Aléatoire selon trades |

### Étape 2 — Élever les cochons

Une fois 2 cochons obtenus :
- Donne **1 carotte / pomme de terre / betterave** à chacun → mode amour → bébé
- Compte ~5 min de croissance pour le bébé adulte

Cible : **8-12 cochons** minimum dans ton enclos pour optimiser le retour par orage.

### Étape 3 — Construire l'enclos + paratonnerre

```
Vue de dessus :
┌──────────────┐
│  Cochons  cochons cochons │
│  cochons  cochons     │
│  cochons  cochons  P  │ ← P = paratonnerre
│  cochons  cochons     │
└──────────────┘
```

- **Enclos** : 5×5 ou 6×6 entouré de barrières
- **Paratonnerre** : posé sur un bloc à **1-2 blocs de hauteur** au-dessus du sol de l'enclos
    - **Pas trop haut** sinon les cochons sont trop loin du point d'impact pour se transformer
    - **Pas au sol** sinon les cochons collent contre

### Étape 4 — Attendre un orage

Les orages sont aléatoires en MC (chaque pluie a une chance de devenir orage). Patience.

`/island keepalive on` pour que ça tourne même offline.

### Étape 5 — La foudre frappe

Quand l'orage arrive et que la foudre tape le paratonnerre, tous les cochons dans un **rayon de ~4 blocs** se transforment en **piglins zombifiés**.

⚠️ **Les piglins zombifiés sont neutres au début, mais agressifs si tu en attaques un (= alerte le groupe).** Prépare-toi :
- Armure (au moins fer si possible)
- Épée
- Pomme dorée enchantée en réserve pour le clutch

### Étape 6 — Tuer les piglins zombifiés

**Drops par kill** (vanilla) :
- 0-1 **pépite d'or** (très courant)
- 0-1 **lingot d'or** (rare, ~5%)
- 0-1 **chair putréfiée**
- Avec Pillage III : drops boostés

**Ratio attendu** :
- ~0.5 pépite d'or par kill en moyenne
- 9 pépites = 1 lingot d'or
- Pour 16 lingots d'or (2 pommes dorées) → environ **160-200 piglins zombifiés tués au total**

C'est beaucoup, mais avec un cycle régulier (orages + reproduction des cochons survivants), tu accumules vite.

## 🥄 Méthode secondaire : fondre le stuff en or (peu efficace)

Les zombies et squelettes nocturnes peuvent spawn avec **équipement en or** (épée en or, casque en or). Quand tu les tues, ils drop parfois leur stuff.

→ Met le stuff au four → **1 pépite d'or** par item fondu.

| Item | Coût original | Récup au four |
|---|---|---|
| Épée en or | 2 lingots (18 pépites) | 1 pépite |
| Casque en or | 5 lingots (45 pépites) | 1 pépite |

**→ Très lossy** (~95% de perte par rapport au matériau original). Recommandé uniquement comme bonus quand tu farms les zombies pour autre chose (fer, par exemple), mais pas comme source principale.

## Stratégie recommandée

```
Phase 1 — Farm de zombies + fer (~300 kills pour ~10 lingots de fer = chaudron + seau)
Phase 2 — Capture 1er cochon + farm carottes/patates (drops zombies)
Phase 3 — Reproduction cochons → enclos de 8-12 cochons
Phase 4 — Paratonnerre + attente orage → transformation en masse
Phase 5 — Kill piglins zombifiés → cycle régulier d'or
Phase 6 — 16 lingots accumulés → 2 pommes dorées → 2 cures de villageois zombies
```

## Astuces

- **Plusieurs enclos** : tu peux faire **2-3 enclos avec paratonnerre** en parallèle pour multiplier le retour par orage
- **Hopper sous la zone de kill** : automatise la collecte des drops piglin zombifié
- **Armure en or** : si tu portes au moins 1 pièce d'armure dorée, les piglins zombifiés ne t'attaquent **pas** spontanément (utile pour les manipuler en sécurité)

## Liens connexes

- [Premier seau d'eau](premier-seau-eau.md) — autre dépendance early game qui demande des zombie kills
- [Émeraudes pour marchand ambulant](emeraudes-marchand.md) — la suite logique : utiliser tes pommes dorées pour cure des villageois zombies
- [Recette : Minerai d'or](../recettes/minerais.md) — utile **après** avoir un stock d'or pour générer plus via Fortune
