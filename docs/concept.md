# Le concept

## Trois dimensions par joueur

Chaque joueur possède **trois dimensions privées** créées à sa première connexion, partageant la même seed aléatoire :

- **Overworld** — `vanillasky:player/<uuid>/overworld`
- **Nether** — `vanillasky:player/<uuid>/nether` (échelle ×8 normale)
- **End** — `vanillasky:player/<uuid>/end`

Personne d'autre n'a accès à tes mondes. Tes constructions, tes farms et ton exploration sont entièrement privés. Les portails t'envoient toujours vers **tes propres dimensions**, jamais vers les dims partagées.

## Indépendance totale

- **Cycle jour/nuit** indépendant — si tu dors, tu passes la nuit, seul.
- **Météo** indépendante — ta pluie ne tombe que chez toi.
- **Sommeil** — pas besoin que tout le serveur dorme pour passer la nuit.
- **Mobs** — ce qui spawn chez toi reste chez toi.
- **Inventaire conservé à la mort** partout sur le serveur — tu gardes ton inventaire quel que soit ta dimension et la cause de mort (vide, mob, void, `/kill`).
- **Combat de l'Ender Dragon** — chaque joueur a son propre Ender Dragon dans son End.

## Un vrai monde, mais vidé

Le générateur de monde vanilla produit les biomes et les structures (villages, monuments, chambres des épreuves, donjons, anciennes cités, forts, vestiges de bastion, forteresses du Nether…), mais leurs blocs sont retirés à la génération.

Les **boîtes englobantes** (bounding boxes, abrégées **BB**) des structures restent enregistrées dans les données du chunk — visibles via un mod client comme **Mini-HUD**, ou repérables d'avance avec ta seed sur **[chunkbase.net](https://www.chunkbase.net)**.

### Exceptions préservées

Les structures ont du contenu spécifique pour le gameplay :

!!! example "Fort (stronghold)"
    Seul l'**anneau de 12 cadres de portail de l'End** est conservé. Tu dois remplir les cadres avec 12 yeux de l'Ender (craftés via poudre de Blaze + perle de l'Ender) pour activer le portail.

!!! example "Ancienne cité"
    Le **cadre central en ardoise des abîmes renforcée** + 1 **Hurleur sculk** avec `can_summon=true` à environ 5 blocs (idéal pour farm Warden).

!!! example "End"
    La **fontaine de sortie** (bedrock + portail) à **Y=60** avec 1 pierre de l'End placée sous chaque bedrock. Pas de torches sur les piliers de bedrock. Pas de piliers d'obsidienne, pas de cristaux de l'End. Le dragon spawn automatiquement à Y=128 dès la création de la dimension.

!!! example "Vestiges de bastion"
    Aucun bloc préservé, mais les **piglins brutes** peuvent spawn dans la BB (s'ajoute aux spawns biomiques normaux : piglins, hoglins, piglins zombifiés).

!!! example "Chambres des épreuves"
    **Générateurs des épreuves** et **coffres-forts** (réguliers + funestes) **préservés**. Le combat se déclenche en cliquant-droit sur un générateur inactif avec un **bâton de Breeze** (voir [Mécaniques](mecaniques/chambres-epreuves.md)).

!!! example "Nether"
    Entièrement vide (les BB des bastions sont enregistrées pour les spawns spéciaux).

## Ton point de départ

Seule **ton île de spawn** (une plateforme losange en herbe + un chêne) flotte dans le vide de l'Overworld. Tout le reste est air — à toi de construire ton monde.

[:material-arrow-right: Découvre ton spawn en détail](spawn.md){ .md-button }
