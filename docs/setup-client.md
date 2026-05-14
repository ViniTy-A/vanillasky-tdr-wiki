# Setup client (recommandé)

Rien n'est imposé côté client : tu peux jouer en vanilla. Mais certains mods rendent l'expérience nettement plus agréable.

Tous les mods listés ci-dessous sont à installer dans le dossier `mods/` de ton client **Fabric 1.21.11**, **pas** sur le serveur. Ils sont **optionnels** : tu peux jouer sans, mais c'est plus confortable avec.

## Mods clients recommandés

### Mini-HUD ⭐ Indispensable

Affiche les boîtes englobantes (BB) des structures cachées dans tes mondes vidés (forts, anciennes cités, vestiges de bastion, etc.).

Le serveur a **Servux** qui pousse les BB automatiquement — il te suffit d'installer Mini-HUD côté client.

[:material-download: Télécharger Mini-HUD](https://modrinth.com/mod/minihud){ .md-button .md-button--primary }

### MaLiLib

Dépendance requise par Mini-HUD (et les autres mods Masa).

[:material-download: Télécharger MaLiLib](https://modrinth.com/mod/malilib){ .md-button }

### Better Advancements

Agrandit la fenêtre des avancements en plein écran et permet de zoomer/scroller à la souris. Très utile pour parcourir les **~90 advancements** de la progression Vanilla Sky.

[:material-download: Télécharger Better Advancements](https://modrinth.com/mod/better-advancements){ .md-button }

### Mod Menu

Ajoute un bouton **« Mods »** dans le menu principal pour configurer tes mods Fabric depuis le jeu (Mini-HUD, etc.).

[:material-download: Télécharger Mod Menu](https://modrinth.com/mod/modmenu){ .md-button }

### Litematica

Pose des **hologrammes** de schémas de construction (formats `.litematic` / `.schematic`) avec liste de matériaux intégrée. Indispensable pour suivre les schemas du wiki — notamment les [tours à mobs](tutoriels/ferme-mobs-sans-eau.md) qui ont leur fichier `.litematic` téléchargeable directement.

[:material-download: Télécharger Litematica](https://modrinth.com/mod/litematica){ .md-button }

!!! warning "Attention à la version"
    Tous ces mods ont plusieurs versions selon ta version Minecraft. **Choisis toujours la version compatible avec ton client** (Fabric **1.21.11** pour TdR). Sur Modrinth, utilise le filtre **Game versions = 1.21.11** + **Loader = Fabric** avant de télécharger.

## Sites utiles

### Modrinth

Plateforme de référence pour télécharger les mods Fabric. Tous les mods ci-dessus s'y trouvent. Tu peux aussi utiliser leur launcher (Modrinth App) qui simplifie la gestion des modpacks.

→ [modrinth.com](https://modrinth.com)

### Chunkbase

Avec ta seed (`/myseed`), tu peux explorer ton monde en 2D : positions des structures, biomes, slime chunks. La même seed s'applique à tes 3 dimensions.

→ [chunkbase.com](https://chunkbase.com)

!!! danger "Attention au typosquat"
    Le vrai site est **chunkbase.com** — le domaine **.net** est un **typosquat** qui sert de fausses alertes antivirus ("Your computer might be infected — Avast"). Ne tape jamais l'URL à la main, utilise toujours un lien direct (`/myseed` te le donne en jeu).

## Activer la ligne biome dans F3

En MC 1.21.x, le F3 utilise un système d'**entries modulaires**. La ligne `Biome: ...` n'est pas activée par défaut. Pour l'activer :

1. En jeu, presse `F3` pour ouvrir le debug screen
2. Tape ensuite **F3+F6** — un écran de config s'ouvre
3. Active l'entry **BIOME** (et autres si tu veux : LIGHT_LEVELS, HEIGHTMAP, etc.)
4. Valide. La ligne biome apparaît maintenant en permanence.

## Configurer Mini-HUD une fois installé

1. Ouvre le config GUI de Mini-HUD (raccourci à configurer dans Controls)
2. Onglet **Renderers** → active **overlayStructureMainToggle**
3. Active les types de structure que tu veux voir : Village, Forteresse, Chambre des épreuves, Vestige de bastion, Ancienne cité, etc.
