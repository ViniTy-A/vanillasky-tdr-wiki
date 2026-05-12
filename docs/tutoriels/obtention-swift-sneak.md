# Tuto — Obtention de Swift Sneak

L'enchantement **Swift Sneak** (Furtivité rapide) permet de marcher à vitesse quasi normale en mode accroupi. En vanilla MC, il ne s'obtient **que** dans les coffres des anciennes cités — donc inaccessible sur TdR puisque les coffres sont vidés.

Sur TdR, on a ajouté une mécanique custom inspirée de **CarpetSkyAdditions** : enchanter **près d'un Warden**.

!!! info "Vidéo à venir"
    Tuto vidéo en cours.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Obtention de Swift Sneak — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen></iframe>
-->

## La mécanique custom TdR

Quand tu utilises une **table d'enchantement** avec **un Warden à ≤12 blocs** de la table :

- L'enchantement **Swift Sneak** est ajouté au pool des enchantements possibles
- Compatible avec : **livres** et **jambières** (cuir, mailles, fer, or, diamant, Netherite)
- Si le coût rollé tombe dans la plage de niveau, swift_sneak peut être sélectionné comme un des 3 enchants proposés

!!! info "Différence avec CSA-Reborn"
    CSA utilise 8 blocs de distance, TdR utilise **12 blocs** (un poil plus permissif vu la taille du Warden).

## Coûts par niveau

| Niveau | minCost | maxCost |
|---|---|---|
| Swift Sneak I | 21 | 71 |
| Swift Sneak II | 28 | 78 |
| Swift Sneak III | 35 | 85 |

!!! warning "Niveau 3 inaccessible direct"
    Les enchantements depuis une table cappent à ~30 niveaux affichés. Swift Sneak III a un minCost de 35, donc **impossible** à obtenir directement à la table. Procédure obligatoire :

    → Obtiens **2 livres Swift Sneak II** puis combine-les sur **enclume** pour produire 1 livre Swift Sneak III.

## Pré-requis

- **1 Warden** à proximité (voir [Mécanique : Hurleur sculk pré-placé](../mecaniques/drops.md#hurleur-sculk-can_summon-pre-place))
- **1 table d'enchantement** (3 obsidienne + 2 diamants + 1 livre)
- **15 étagères** (bookshelves) autour de la table pour avoir des enchantements niveau 30
- **30 niveaux d'XP** par tentative d'enchantement
- **1 lapis-lazuli** par tentative
- **Livres** ou **jambières** à enchanter
- Équipement de combat solide (Netherite Protection IV recommandé pour survivre près du Warden)

## Étape 1 — Localiser une ancienne cité

`/myseed` + [chunkbase.net](https://chunkbase.net) → Structure Finder → "Ancient City". Construis un pont jusqu'aux coordonnées.

Sur TdR, **le hurleur sculk au centre de l'ancienne cité est pré-placé** avec `can_summon=true` — il sert directement à spawn le Warden.

## Étape 2 — Construire ta zone d'enchantement "sécurisée"

Plus complexe que ça en a l'air à cause du Warden et de son sonic boom.


## Étape 3 — Spawner le Warden

Saute / casse des blocs / fais du bruit autour du hurleur **4 fois consécutivement** dans un rayon de 16 blocs → le hurleur invoque un Warden.

!!! tip "Effet Darkness"
    Tu vas recevoir l'effet **Darkness** pendant les activations. Bois du **lait** pour l'annuler si ça te gêne (ou attends que ça passe seul).

## Étape 4 — Enchanter

Une fois le Warden spawné et à ≤12 blocs de ta table :

1. Pose un **livre** ou une **paire de jambières** sur la table
2. Ajoute 1-3 **lapis-lazuli** et au moins 30 niveaux d'XP
3. Regarde les 3 enchants proposés — un d'entre eux peut être **Swift Sneak I, II.
4. Si swift_sneak n'apparaît pas dans les 3 propositions, **annule** (clique pas), enchante autre chose pour re-roller, et recommence

**Probabilité** : random, dépend du roll de coût. Compte plusieurs essais.

## Étape 5 — Obtenir Swift Sneak III

Le niveau 3 ne sort jamais directement de la table (capé à 30, minCost III = 35).

**Procédure** :
1. Enchante jusqu'à obtenir **2 livres Swift Sneak II**
2. Sur enclume, combine **livre Swift Sneak II + livre Swift Sneak II** → 1 livre Swift Sneak III
3. Applique ce livre sur tes jambières avec une enclume.

## Astuces

- **Anti-Warden** : place ta plateforme et reste accroupi quand tu approches. Le Warden détecte les vibrations + les odeurs.
- **Multi-essais** : prépare plein de livres + lapis avant de spawn le Warden, comme ça tu n'as pas à re-spawn pour plusieurs essais
- **Warden contre cri sonique** : si tu es à 5 blocs et au-dessus, le Warden ne peut pas te toucher en mêlée mais il peut te frapper avec son cri sonique.

## Bonus — Avantages de Swift Sneak

- Niveau **I** : marche à 30% de la vitesse normale en accroupi
- Niveau **II** : marche à 60% de la vitesse normale en accroupi
- Niveau **III** : marche à 90% de la vitesse normale en accroupi



## Liens connexes

- [Mécanique : Hurleur sculk pré-placé](../mecaniques/drops.md#hurleur-sculk-can_summon-pre-place)
- [Mécanique : Catalyseur sculk via Warden](../mecaniques/mobs.md#catalyseur-sculk-via-warden)
- [Mécanique : Éclat d'écho via sonic boom Warden](../mecaniques/mobs.md#eclat-decho-via-warden-sonic-boom)
