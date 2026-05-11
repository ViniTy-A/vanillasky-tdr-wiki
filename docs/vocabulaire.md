# Vocabulaire

Petit lexique des termes techniques utilisés dans ce wiki. Si tu vois un mot que tu ne connais pas dans une autre section, il est probablement défini ici.

## BB (bounding box)

Boîte englobante invisible qui marque l'emplacement et le volume d'une structure (fort, ancienne cité, vestige de bastion, etc.).

Même si tous les blocs de la structure sont retirés par le mod, la **BB reste enregistrée** dans les données du chunk.

**Pour la voir en jeu** : installe **Mini-HUD** côté client (le serveur a Servux qui pousse les données automatiquement), active *overlayStructureMainToggle* et le type de structure voulu.

**Pour la repérer d'avance** : entre ta seed sur **chunkbase.net** (Structure Finder).

## Seed

Nombre unique qui détermine entièrement la génération de ton monde (positions des biomes, structures, minerais, etc.).

Tape `/myseed` pour la récupérer. À copier sur **chunkbase.net** pour explorer ton monde en 2D avant de partir.

## Dim / Dimension

Un monde Minecraft séparé. Tu en as **3 privées** : ton Overworld, ton Nether et ton End. Personne d'autre n'a accès à tes dims.

## Tick

Unité de temps de Minecraft. **20 ticks = 1 seconde**.

La plupart des mécaniques (croissance des plantes, drops, ticks de bloc) sont rythmées en ticks.

## Random tick

Tick aléatoire qui ne s'applique qu'à certains blocs (cultures qui poussent, herbe qui se propage, feuilles qui pourrissent).

En vanilla, ~3 random ticks/seconde par chunk, avec une chance de tomber sur un bloc précis. Pour qu'ils déclenchent en AFK, il faut que le chunk soit chargé.

## Chunk

Section verticale de **16×16 blocs** (avec toute la hauteur du monde). MC charge le monde par chunks autour du joueur.

Un chunk « chargé » est un chunk qui tick activement.

## Force-load

Mécanisme qui maintient un chunk chargé même si aucun joueur n'est à proximité. Indispensable pour qu'une farm AFK continue de tourner quand tu es loin.

Sur ce serveur, les seuls chunks force-loaded sont les chunks de spawn de chaque dim vanillasky ; pour le reste, utilise `/island keepalive on` qui garde tes 3 dims chargées même offline.

## Keepalive

Option custom du mod (`/island keepalive on|off`). Quand activé, tes 3 dims restent chargées même quand tu te déconnectes — tes farms AFK continuent.

## AFK farm

Farm conçue pour produire automatiquement des ressources pendant que tu es immobile (ou même offline avec keepalive).

Exemples : farm d'or sur portails Nether, farm de Warden sur l'ancienne cité, farm de coraux.

## Générateur / Générateur des épreuves

Bloc qui fait apparaître des mobs périodiquement. Le **générateur classique** a une cage avec un mob miniature qui tourne.

Le **générateur des épreuves** (1.21) est dans les chambres des épreuves : il déclenche des vagues de mobs et fournit une clé des épreuves + récompenses.

## Coffre-fort / Coffre-fort funeste

Bloc dans les chambres des épreuves qui s'ouvre avec une **clé des épreuves** et donne une récompense (potions, lingots, parfois des disques rares ou motifs de bannière).

Variante **funeste** (liée à Mauvais présage) avec du loot plus rare.

## Fortune

Enchantement qui augmente le nombre de drops de certains blocs minés (minerais, feuilles, etc.). **3 niveaux**.

## Toucher de soie (Silk Touch)

Enchantement qui fait drop le bloc tel quel au lieu de son contenu habituel. Utile pour récolter de la glace, des minerais bruts, etc.

## Marchand ambulant (wandering trader)

Mob qui spawn aléatoirement avec 2 lamas. Son cycle de spawn est **indépendant par joueur** (chaque dim a son propre cycle).

Source initiale des coraux, des fleurs hautes, des pousses d'arbre.

## Troc (bartering)

Échange avec un piglin : tu jettes un lingot d'or à ses pieds, il te jette un objet aléatoire en retour. Source des perles de l'Ender, obsidienne pleureuse, roche noire dorée, et du disque Pigstep en BB de bastion.

## Creeper chargé

Creeper qui a été frappé par un éclair (ou un canal de Trident Canalisation). Son explosion est plus grosse, et tuer un mob avec lui drop sa **tête** (creeper, squelette, zombie, piglin, Ender Dragon).

## OP / Opérateur

Joueur avec privilèges admin sur le serveur. Niveau 2+ donne accès aux commandes gamemaster (`/gamemode`, `/summon`, `/tp`, etc.). Géré côté serveur.

## Mini-HUD

Mod client (par **masa.dev**) qui affiche en jeu les BB des structures, les niveaux de lumière, les chunks, et plein d'autres infos utiles. Dépend de **Servux** côté serveur pour les données structure.

## Servux

Mod serveur qui pousse aux clients Mini-HUD les données nécessaires (BB des structures, etc.). Installé sur le serveur. **Ne force aucun mod côté joueur**.

## Chunkbase

Site web ([chunkbase.net](https://chunkbase.net)) qui visualise un monde Minecraft à partir de sa seed.

Apps utiles : Biome Finder, Structure Finder, Slime Chunks. Pas besoin d'installer quoi que ce soit.

## Datapack

Pack de données qui modifie le gameplay (recettes, advancements, loot tables, fonctions). Le mod en embarque un automatiquement (`vanillasky`) — visible via `/datapack list`.

## F3

Touche pour ouvrir le **debug screen** de Minecraft. Affiche position, biome, FPS, chunks chargés, etc.

En MC 1.21.x, certaines lignes sont modulaires (à activer via **F3+F6**).
