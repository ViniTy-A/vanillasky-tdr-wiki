# Roadmap

## Features actuelles déjà en place

### Mondes et dimensions
- [x] Overworld + Nether + End par joueur (3 dimensions privées)
- [x] Routage automatique des portails vers les dimensions du joueur
- [x] Inventaire conservé universellement à la mort

### Worldgen et structures
- [x] Vraies structures vanilla générées mais blocs vidés
- [x] Fort préservé (anneau de cadres de portail de l'End)
- [x] Ancienne cité préservée (cadre central + hurleur sculk `can_summon`)
- [x] Vestiges de bastion : spawns de piglins brutes
- [x] End : fontaine + pierre de l'End sous chaque bedrock
- [x] Chambres des épreuves : générateurs des épreuves + coffres-forts préservés (masse, bâton de Breeze, charge de vent, noyau lourd, ornements boulons/tourbillons, disques Creator/Precipice)

### Plateformes de portail
- [x] Plateforme Nether 8 blocs (nylium carmin/biscornu/netherrack selon biome)
- [x] Plateforme retour côté Overworld

### Recettes custom
- [x] Recettes minerais en croix (Overworld + abîmes + Nether)
- [x] Recettes armures de cheval (motif H)
- [x] Recettes armures de nautile (motif coquille d'escargot)
- [x] Recette modèle de forge — mise à niveau Netherite
- [x] Baies lumineuses (sans forme)
- [x] Haut fourneau : diorite → calcite, andésite → tuf

### Mécaniques de ressources
- [x] Érosion + propagation des coraux
- [x] Diamant via enclume + bloc de charbon
- [x] Mycélium via énorme champignon
- [x] Buisson mort via pousse sur sable
- [x] Buisson via fiole d'eau sur buisson mort
- [x] Baies sucrées via renards
- [x] Tête de dragon via creeper chargé
- [x] Druse d'améthyste via pattern de géode
- [x] Allay via Vex (séquence de 5 notes sur blocs musicaux)
- [x] Araignée des cavernes via pomme de terre empoisonnée
- [x] Pétales roses via cuisson feuilles de cerisier
- [x] Plante de chorus auto sur portails de l'End
- [x] Hautes herbes / grande fougère via enderman porteur

### Mobs et drops
- [x] Drops creeper liés à la BB de structure (Pigstep, Otherside, fragment 5, 11, Creator, Creator Music Box, Precipice)
- [x] Charge de chèvre → bloc de verrue du Nether (1-2 verrues)
- [x] Toile d'araignée via araignée chevauchée (1 par spawn)
- [x] Fleur sporifère via feuille d'azalée fleurie (Fortune-scaled)
- [x] Roche noire dorée via troc piglin (~1%)
- [x] Élytres via endermite (chute lente + lévitation)
- [x] Marchand ambulant à chameau (désert + variants badlands)
- [x] Blaze → Breeze (passage Nether → Overworld)
- [x] Fleurs hautes via marchand ambulant (tournesol, lilas, rosier, pivoine)
- [x] Éclat d'écho via sonic boom Warden sur chauve-souris/dauphin
- [x] Pomme d'or enchantée via cadeau du matin de chat
- [x] Œuf de renifleur via noyé porteur + œufs de tortue
- [x] Lichen luminescent via foudre sur lianes
- [x] Cœur de la mer via dauphin
- [x] Shulker renouvelable via re-spawn dragon
- [x] Motif de bannière piglin via zoglin
- [x] Catalyseur sculk via Warden
- [x] Terre des âmes via feu de camp des âmes
- [x] Chameau via marchand ambulant désert
- [x] Éponge via gardien ancestral

### Chambres des épreuves (strict CSA-Reborn)
- [x] Générateurs des épreuves bloqués INACTIVE par défaut
- [x] Activation uniquement via clic-droit bâton de Breeze
- [x] Loot des coffres-forts rebalancé (sans ornements d'armure ni disques)
- [x] Tessons tourbillon / rafaleur / hache dans coffres-forts uniques

### Succès Tier 3 (challenges)
- [x] Conquérant de la foudre → Ornement des boulons
- [x] Maîtrise du flux → Ornement des tourbillons
- [x] Conquérant du bastion → motif de bannière piglin (100 brutes tuées)
- [x] ~12 succès Tier 3 supplémentaires (trim advancements + autres)

### Progression
- [x] 93 succès de progression alignés sur CSA-Reborn
- [x] Activation générateur des épreuves (strict via clic bâton)
- [x] Bâton de Breeze (inventaire)
- [x] Disques chambre des épreuves (Precipice + Creator)
- [x] Armure de nautile en diamant
- [x] Buisson (rehydratation)
- [x] Cœur de grinceur
- [x] Swift Sneak via table d'enchantement avec Warden à ≤12 blocs

### Commandes serveur
- [x] `/myseed` + alias FR `/maseed`
- [x] `/island keepalive on|off`
- [x] `/recompense` (récompenses en attente)
- [x] `/reset` + alias FR `/recommencer` (avec confirmation 2 étapes + cooldown 15 min)
- [x] Commandes admin OP : `/god`, `/fly`, `/heal`, `/feed`

### Infrastructure
- [x] Compteur de morts dans la tab list (scoreboard objective)
- [x] Mod custom **vanillasky** 0.1.0 (Fabric 1.21.11)
- [x] Datapack `vanillasky` embarqué dans le mod

## En cours / À venir

### Doc et accessibilité
- [x] Wiki MkDocs Material en ligne (ce site)
- [x] Traductions FR_FR / FR_CA / EN_US des advancements (108/108 dans chaque langue, termes vanilla MC FR Java vérifiés)
- [ ] Tutoriels vidéo — textes rédigés, **enregistrements vidéo en cours** (descente Y=-64, druse d'améthyste, etc.)

### Features potentielles
- [x] Système d'enchères entre joueurs (`/ah` avec GUI, persistence, mailbox, offres)
- [x] Visites entre îles (`/island invite|uninvite|visitors|public on|off` + alias FR `/ile inviter|désinviter|visiteurs|public`)
- [ ] Stats globales sur le wiki (joueurs actifs, mondes générés, etc.)

## Date d'ouverture du serveur

🎯 **1er juillet 2026**

D'ici là, le focus est sur :
1. Finaliser les **enregistrements vidéo** des tutos (textes déjà rédigés)
2. Tests stress avec 20 joueurs simultanés
