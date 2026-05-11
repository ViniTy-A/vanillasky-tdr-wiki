# Tuto — Activer un générateur des épreuves avec un bâton de Breeze

Sur TdR, les **générateurs des épreuves** sont volontairement bloqués en mode strict CSA-Reborn : ils ne s'activent **jamais tout seuls**, peu importe combien de joueurs sont dans le rayon de détection vanilla.

Le **seul** moyen de démarrer un combat est le clic-droit avec un **bâton de Breeze**.

!!! info "Vidéo à venir"
    Enregistrement vidéo à venir.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Activation générateur des épreuves" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen></iframe>
-->

## Pré-requis

- ≥1 **bâton de Breeze** (voir [tuto Blaze → Breeze](blaze-vers-breeze.md))
- Localisation d'une **chambre des épreuves** (`/myseed` + chunkbase.net)
- Équipement de combat solide (armure diamant + Netherite si possible, épée diamant minimum)
- Nourriture (pomme dorée, steaks)
- Bouclier pour parer les attaques

## Étape 1 — Atteindre la chambre des épreuves

1. Identifie la BB sur chunkbase
2. Construis un pont vers les coordonnées
3. Mine vers le bas pour accéder à l'intérieur (les chambres sont souterraines)

!!! tip "Pré-construction"
    Construis ta zone de combat avant d'activer le générateur. Les mobs spawnent dans un rayon défini autour, donc place tes blocs pour limiter les angles d'attaque.

## Étape 2 — Identifier un générateur des épreuves

Les générateurs des épreuves sont des **blocs noirs avec une cage de cuivre verte** au centre. Deux variants :

- **Générateur des épreuves** (régulier) — base en cuivre
- **Générateur des épreuves funeste** (ominous) — base plus sombre

Ils sont **INACTIVE** par défaut (pas d'animation, pas de mobs qui sortent). Sans bâton de Breeze, ils resteront éternellement comme ça sur TdR.

## Étape 3 — Activer avec le bâton

1. Sélectionne ton **bâton de Breeze** dans la barre d'inventaire
2. Pointe le générateur, **clic-droit**
3. Tu vois :
    - Particules d'activation autour du bloc
    - Son d'activation (ominous sound)
    - Message en barre d'action : *« Générateur des épreuves activé avec un bâton de Breeze. »*
4. **1 bâton est consommé** (sauf en créatif)
5. Le générateur passe à `WAITING_FOR_PLAYERS` puis très vite à `ACTIVE` → début du combat

!!! warning "Bonne main"
    Si le bâton n'est pas exactement dans la main qui clique-droit (main droite par défaut), ça ne marche pas. Sélectionne-le bien dans le hotbar.

## Étape 4 — Combattre les vagues

Le générateur produit des vagues de mobs (le type dépend du générateur, varie selon la chambre) :

- Squelettes, zombies, araignées (généraux)
- Stray, Husk, Cave Spider (variantes)
- Slimes
- Breeze (pour les ominous parfois)

Reste mobile, combats à distance quand possible, mange régulièrement.

## Étape 5 — Récolter la clé des épreuves

Une fois toutes les vagues vaincues, le générateur drop une **clé des épreuves** (ou **clé des épreuves funeste** si c'était un ominous).

Utilise la clé pour ouvrir le **coffre-fort** (ou **coffre-fort funeste**) à proximité.

## Étape 6 — Loot rebalancé

Voir [Loot des coffres-forts](../mecaniques/chambres-epreuves.md#loot-des-coffres-forts-rebalance-csa-reborn-style) pour le détail de ce qui peut sortir.

!!! warning "Pas d'ornements d'armure"
    Sur TdR, les **Ornements des boulons** et **Ornements des tourbillons** ne sont **plus** dans les coffres-forts. Ils s'obtiennent via les challenges Tier 3 « Conquérant de la foudre » et « Maîtrise du flux » à la place.

## Astuces

- **Stock plusieurs bâtons** : chaque activation consomme 1 bâton, prévois-en 3-4 avant de t'engager pour répéter plusieurs générateurs dans la même chambre
- **Variant funeste** : utilise une **bouteille de mauvais présage** (gagnée en tuant un porteur de bannière de raid) avant d'activer un générateur funeste — le loot ominous est plus rare/intéressant
- **Plusieurs joueurs** : le combat scale avec le nombre de joueurs proches (plus de joueurs = plus de mobs par vague)

## Liens connexes

- [Mécanique : Générateur via bâton de Breeze](../mecaniques/chambres-epreuves.md#generateur-des-epreuves-active-via-baton-de-breeze-strict)
- [← Conversion Blaze → Breeze](blaze-vers-breeze.md)
- [Conquérant de la foudre →](conquerant-foudre.md)
