# Tuto — Obtention de Swift Sneak

L'enchantement **Swift Sneak** (Furtivité rapide) permet de marcher à vitesse quasi normale en mode accroupi. En vanilla MC, il ne s'obtient **que** dans les coffres des anciennes cités — donc inaccessible sur TdR puisque les coffres sont vidés.

Sur TdR, on a ajouté une mécanique custom inspirée de **CarpetSkyAdditions** : enchanter **près d'un Warden**.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 0.3rem; margin: 1.5rem 0; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
  <iframe
    src="https://www.youtube-nocookie.com/embed/WFve9dPyz9Y?rel=0"
    title="Obtention de Swift Sneak — Vanilla Sky TdR"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0;"
    loading="lazy"
    allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen></iframe>
</div>

<p style="text-align: center; margin-top: -0.5rem; font-size: 0.85em; opacity: 0.7;">
  <a href="https://youtu.be/WFve9dPyz9Y" target="_blank" rel="noopener">▶ Regarder sur YouTube</a>
  · Le tuto écrit ci-dessous reprend les mêmes étapes en référence
</p>

## La mécanique custom TdR

Quand tu utilises une **table d'enchantement** avec **un Warden à ≤12 blocs** de la table :

- L'enchantement **Swift Sneak** est ajouté au pool des enchantements possibles
- Compatible avec : **livres** et **jambières** (cuir, mailles, fer, or, diamant, Netherite)
- Si le coût rollé tombe dans la plage de niveau, swift_sneak peut être sélectionné comme un des 3 enchants proposés

## Coûts par niveau

Sur TdR, les `minCost` de Swift Sneak ont été **abaissés** par rapport à vanilla pour rendre l'enchantement accessible directement depuis une table d'enchantement (sans devoir obligatoirement combiner deux livres L2 sur enclume).

| Niveau | minCost (TdR) | minCost (vanilla) | maxCost |
|---|---|---|---|
| Swift Sneak I | **18** | 25 | 75 |
| Swift Sneak II | **24** | 50 | 100 |
| Swift Sneak III | **30** | 75 | 125 |

!!! tip "Niveau 3 accessible directement"
    Avec un `minCost III = 30`, Swift Sneak III est **dans la plage** d'une table maxée (15 bookshelves → 30 niveaux affichés). C'est RNG-dépendant — il faut que le roll tombe dans `[30, 125]` ET que swift_sneak soit pioché parmi les 3 enchants proposés — mais c'est réalisable en une seule tentative.

    → Le combine enclume L2+L2 reste une **option** plus consistante si tu veux pas dépendre du RNG.

## Pré-requis

- **1 Warden** à proximité (voir [Mécanique : Hurleur sculk pré-placé](../mecaniques/drops.md#hurleur-sculk-can_summon-pre-place))
- **1 table d'enchantement** (3 obsidienne + 2 diamants + 1 livre)
- **15 étagères** (bookshelves) autour de la table pour avoir des enchantements niveau 30
- **30 niveaux d'XP** max par tentative d'enchantement
- **3 lapis-lazuli** max par tentative
- **Livres** ou **jambières** à enchanter
- Équipement de combat solide (Netherite Protection IV recommandé pour survivre près du Warden)

## Étape 1 — Localiser une ancienne cité

`/myseed` + [chunkbase.com](https://chunkbase.com) → Structure Finder → "Ancient City". Construis un pont jusqu'aux coordonnées.

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
3. Regarde les 3 enchants proposés — un d'entre eux peut être **Swift Sneak I, II ou III** (selon le coût rollé et la chance).
4. Si swift_sneak n'apparaît pas dans les 3 propositions, **annule** (clique pas), enchante autre chose pour re-roller, et recommence

**Probabilité** : random, dépend du roll de coût. Compte plusieurs essais.

## Étape 5 — Obtenir Swift Sneak III

Deux voies possibles :

**Voie directe (RNG)** — depuis une table maxée à 30 niveaux, Swift Sneak III peut sortir tel quel. Rapide quand ça tombe, mais le pool d'enchants au niveau 30 contient beaucoup de candidats donc il faut souvent re-roller.

**Voie enclume (consistante)** — si le RNG te frustre :

1. Enchante jusqu'à obtenir **2 livres Swift Sneak II**
2. Sur enclume, combine **livre Swift Sneak II + livre Swift Sneak II** → 1 livre Swift Sneak III
3. Applique ce livre sur tes jambières avec une enclume.

## Astuces

- **Anti-Warden** : place ta plateforme et reste accroupi quand tu approches. Le Warden détecte les vibrations + les odeurs.
- **Multi-essais** : prépare plein de livres + lapis avant de spawn le Warden, comme ça tu n'as pas à re-spawn pour plusieurs essais
- **Warden contre sonic boom** : à 5 blocs et au-dessus, le Warden ne peut pas te toucher en mêlée mais il déclenchera son **sonic boom** à la place. Le sonic boom **traverse tous les blocs** (y compris l'obsidienne) et **ne nécessite pas de ligne de vue**. La seule vraie défense est de rester **hors de la portée de ~20 blocs** du Warden quand tu n'enchante pas — par exemple en restant en hauteur loin de lui et en redescendant uniquement pour les ~5s d'enchant.

## Bonus — Avantages de Swift Sneak

- Niveau **I** : marche à 30% de la vitesse normale en accroupi
- Niveau **II** : marche à 60% de la vitesse normale en accroupi
- Niveau **III** : marche à 90% de la vitesse normale en accroupi



## Liens connexes

- [Mécanique : Hurleur sculk pré-placé](../mecaniques/drops.md#hurleur-sculk-can_summon-pre-place)
- [Mécanique : Catalyseur sculk via Warden](../mecaniques/mobs.md#catalyseur-sculk-via-warden)
- [Mécanique : Éclat d'écho via sonic boom Warden](../mecaniques/mobs.md#eclat-decho-via-warden-sonic-boom)
