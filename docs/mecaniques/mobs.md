# Mécaniques mobs

## Baies sucrées (via renard)

Un **renard** qui spawn a 20% de chance d'avoir des baies sucrées dans la gueule (tu les lui voles ou tu tues le renard).

## Seau de lave (via Héros du village)

Gagne un raid pour obtenir l'effet **Héros du village**. Pendant que l'effet est actif, **trois professions de villageois** peuvent te lancer un seau de lave en cadeau (chance ~14% par gift, le pool gift est rolled toutes les ~5 min de Héros) :

- **Armurier**
- **Forgeron d'armes**
- **Forgeron d'outils**

Aucune autre profession ne donne de lave. L'effet Héros dure **60-80 minutes** (durée fixe selon la difficulté) — reste à proximité de tes villageois pendant ce temps pour maximiser le nombre de gifts roll.

## Tête de dragon (via creeper chargé)

Tue l'**Ender Dragon** avec un **creeper chargé** (explosion directe). La dernière source de dégâts doit être le creeper.

**En pratique** :
1. Amène le dragon à bas PV
2. Attire un creeper sur la plateforme de spawn
3. Frappe-le par la foudre (paratonnerre + orage, ou trident avec Canalisation) pour le rendre chargé
4. Laisse-le exploser sous le dragon

## Marchand ambulant à dos de chameau

Quand un marchand ambulant spawn dans un biome **désert** OU dans une variante **badlands** (badlands, badlands érodées, badlands boisées), il apparaît directement **monté sur un chameau apprivoisé**.

C'est le **seul moyen** d'obtenir un chameau dans le serveur (pas de spawn naturel dans les dims voidées).

**Récupération** : attaque le marchand pour le démonter (ou attends le timer de despawn ~40 min), puis clic-droit sur le chameau pour monter dessus → succès `ride_camel`. Le chameau est tamed donc accepte ta première interaction sans bond.

## Fleurs hautes (via marchand ambulant)

Le marchand ambulant vend désormais les **4 fleurs hautes** en tier 1 :

| Fleur | Coût |
|---|---|
| Tournesol | 1 émeraude |
| Lilas | 1 émeraude |
| Rosier | 1 émeraude |
| Pivoine | 1 émeraude |

**12 trades disponibles** par marchand spawn. Mécanique inspirée de Bedrock Edition + CSA-Reborn.

Sans cette injection de trade (mixin `WanderingTraderTradesMixin`), ces 4 fleurs sont totalement inaccessibles en survie skyblock — vanilla ne les drop pas et elles ne sont pas craftables.

Les fleurs hautes débloquent aussi : 2× pétale rose et autres teintures via crafting (lilas → 2 teintures magenta, tournesol → 2 teintures jaunes, etc.), poudre d'os via composteur de fleurs.

## Blaze → Breeze (passage Nether → Overworld)

Mécanique custom inspirée de CSA-Reborn. Quand un **Blaze** traverse un portail Nether et arrive dans une dimension Overworld (la tienne ou la master), il est **automatiquement converti en Breeze**.

**Procédure** :
1. Capture un Blaze dans ton Nether (ils spawnent dans la BB de forteresse)
2. Lasse-le et amène-le à ton portail Nether
3. Fais-le passer côté Overworld → conversion instantanée en Breeze (santé proportionnelle préservée)
4. Tue le Breeze pour récupérer un **Bâton de Breeze** (et autres drops vanilla)

!!! info "Blaze nommés"
    Les Blaze nommés (avec étiquette) ne sont **pas** convertis (pour qu'on puisse les garder en pet). Conversion fonctionne dans les 2 sens géographiquement : depuis n'importe quel Nether (vanilla ou per-player) vers n'importe quel non-Nether.

!!! tip "À quoi sert le bâton de Breeze ?"
    Le bâton de Breeze est le **seul moyen** d'activer un **générateur des épreuves** dans les chambres des épreuves — l'auto-activation par proximité de joueur est désactivée sur ce serveur. Clic-droit sur un générateur inactif avec un bâton en main pour démarrer le combat (consomme 1 bâton par activation). Voir [Chambres des épreuves → Générateur activé via bâton de Breeze](chambres-epreuves.md#generateur-des-epreuves-active-via-baton-de-breeze-strict).

## Élytres (via endermite)

Tue une **endermite** par toi-même (pas par un autre mob), pendant qu'**elle** est sous les effets **Chute lente** ET **Lévitation** simultanément. Drop 1 paire d'élytres.

**Pratique** : laisse un shulker la viser (le projectile applique Lévitation pendant 10s), puis lance-lui une potion jetable de Chute lente, et tue-la pendant que les 2 effets sont actifs sur elle.

## Ender Dragon (et respawn)

Active le portail de l'End de ton fort (12 yeux de l'Ender). Tu atterris dans **ton End** avec ton dragon à toi.

**Re-respawn possible** : pose 4 **cristaux de l'End** sur les 4 faces cardinales (N/S/E/O) du bedrock central du portail de sortie. Chaque cristal coûte 7 verre + 1 larme de Ghast + 1 perle de l'Ender → **28 verre + 4 larmes + 4 perles** au total pour respawner le dragon.

## Verrue du Nether (renouvelable, via chèvre)

Une **chèvre** qui charge sur un **bloc de verrue du Nether** le casse et drop **1-2 verrues du Nether**.

Mécanisme actif uniquement avec `mobGriefing=true`.

!!! tip "Astuce"
    Utilise une **chèvre beuglante** (charge plus souvent) et place un bloc dans la trajectoire de sa charge vers une cible vivante.

## Toile d'araignée (via araignée chevauchée)

Tue toi-même une **araignée chevauchée** (squelette monté sur une araignée). Le **PREMIER** des deux à mourir drop **1 toile d'araignée**, à condition que l'autre soit encore vivant. Le second mort ne drop rien.

**Kill joueur uniquement** — un mob qui tue la créature ou la chute/lave ne déclenche pas le drop. Donc **1 toile par araignée chevauchée spawn**, max.

## Roche noire dorée

Troc avec un piglin (jette un lingot d'or). Probabilité **~1.09%** par troc (weight 5 sur 459 total). Drop **1-3 roches noires dorées** à chaque trigger.

## Allay (depuis Vex)

Approche un **Vex** à moins de 16 blocs et joue la séquence de 5 notes **C – E – G – C(octave) – G** (notes 0, 4, 7, 12, 7) sur des **blocs musicaux**.

L'instrument importe peu, seule la note compte.

Les notes correctes font apparaître des cœurs ; une mauvaise note remet le compteur à zéro (particules crit). Au 5ème succès → conversion en **Allay**.

## Araignée des cavernes (via pomme de terre empoisonnée)

**Clic droit** sur une araignée normale avec une **pomme de terre empoisonnée** en main. La pomme de terre est consommée et l'araignée se transforme en araignée des cavernes.

## Œuf de renifleur (chaîne complète)

### Étape 1 — Obtenir des œufs de tortue

Trouve une **plage** (biome Plage — les tortues y spawnent naturellement sur le sable). Capture/élève 2 tortues, donne 1 **herbe aquatique** à chacune → reproduction. La tortue rentre vers sa plage de naissance, creuse, pond **1 à 4 œufs** sur le sable.

### Étape 2 — Repérer un noyé porteur

Sur le serveur, **1% des noyés** qui spawnent ont un **œuf de renifleur** dans leur **main secondaire** (visible quand tu les approches : petit œuf vert tacheté tenu à gauche du corps).

!!! warning "Drop chance = 0"
    Tuer le noyé ne donne **jamais** l'œuf, il faut le forcer à le « planter » via les œufs de tortue.

### Étape 3 — Laisser le noyé casser un œuf de tortue

Place les œufs de tortue dans une zone que le noyé peut atteindre (pas trop loin de l'eau). Les noyés et zombies ont une IA qui les pousse à détruire les œufs de tortue.

Quand un noyé porteur active son objectif `RemoveBlockGoal` sur un de tes œufs de tortue et finit l'animation de destruction, l'emplacement du **œuf de tortue détruit** devient un **bloc d'œuf de renifleur** (et la main secondaire du noyé est consommée).

!!! note "Subtilité technique"
    Normalement les zombies/noyés cassent aussi les œufs de tortue en marchant dessus (vanilla, via `destroyEgg` au moment du trample). Le mixin `TurtleEggBlockMixin` annule ce chemin pour les noyés porteurs d'œuf de renifleur — pour qu'ils ne « gâchent » pas leur œuf en piétinant. Ils sont forcés de passer par l'objectif goal-driven.

### Étape 4 — Récolter et faire éclore

Mine le bloc œuf de renifleur (drop garanti, pas besoin de Toucher de soie). Pose-le où tu veux. Pour **accélérer l'éclosion** :

- Sur un **bloc de mousse** → éclosion en ~20 min
- Sur n'importe quel autre bloc → ~5h

### Étape 5 — Sable suspect via renifleur

Une fois adulte, le renifleur creusera des trous dans le **sable** ou le **gravier**. **Quand il fouille à l'intérieur d'une structure d'archéologie** (pyramide du désert, ruines océaniques chaudes/froides, ruines du sentier), 10% de chance par fouille de convertir le bloc en **sable suspect** ou **gravier suspect** avec la table de butin de la structure.

Brosse-le ensuite avec un **pinceau** pour récupérer les tessons de poterie.

## Pomme d'or enchantée (via chat)

Apprivoise un **chat** (avec un poisson cru), couche-toi dans un lit à proximité (≤16 blocs). Au réveil, le chat a une chance de poser un **cadeau du matin** sur le lit.

Le pool inclut : peau de lapin, ficelle, poulet, chair putréfiée, plume, membrane de phantom (poids 16 chacun) **et** pomme d'or enchantée (poids 1). **Probabilité par cadeau : ~1%**.

!!! tip "Multiplier les chances"
    Plusieurs chats à côté = plusieurs cadeaux.

## Cœur de la mer (via dauphin)

Donne un **poisson** (morue, saumon, poisson tropical) à un **dauphin** sauvage en lui jetant l'item au sol — il le ramasse. Une fois nourri, suis-le au-dessus d'un fond de **sable** ou **gravier** en eau.

Toutes les secondes, s'il est en eau au-dessus du bon fond, il joue son animation de fouille (particules de sable/gravier détruit) avec **5% de chance** de remonter un **cœur de la mer** dans sa gueule. Il le laisse tomber peu après.

Un poisson = un essai (l'état « nourri » est consommé).

## Shulker (renouvelable)

Tue ton **Ender Dragon** une première fois. Re-respawn le dragon avec 4 cristaux de l'End (sur les 4 faces cardinales du bedrock central du portail de sortie).

Tue-le une **seconde fois** → un **shulker** apparaît au sommet du pilier de bedrock central, 4 blocs au-dessus du portail. Tue-le pour valider le succès Tier 3 et récupérer une **carapace de Shulker**.

Le mécanisme est répétable indéfiniment : à chaque re-tue d'un dragon respawné, un nouveau shulker apparaît.

## Catalyseur sculk (via Warden)

Fais déclencher un **Warden** via un hurleur sculk (4 activations consécutives). Laisse le Warden tuer plusieurs mobs hostiles à proximité — chaque kill propage la **sculk** autour du cadavre via les particules d'XP.

Avec une chance, des **catalyseurs sculk** apparaissent dans la propagation. Mine-les avec une **pioche enchantée Toucher de soie** pour les récupérer.

!!! tip "Astuce"
    Amène plusieurs zombies/squelettes dans la zone du Warden pour multiplier les chances.

## Motif de bannière piglin (museau, via zoglin)

Tue un **zoglin** par toi-même (peu importe la dimension : Nether, Overworld ou End — le drop s'applique partout, le critère est `killed_by_player` sans condition de dim).

**10% de chance par kill** de drop un motif de bannière piglin (motif « museau »).

Les zoglins sont des **hoglins** qui ont passé plus de 15 secondes hors du Nether — pour en faire spawn : ramène un hoglin (mob du Nether) via ton portail vers ton Overworld, attends 15s, il se transforme en zoglin. Tue-le. Répète jusqu'au drop.

## Chameau (via marchand ambulant)

Le **marchand ambulant** spawn dans un biome **désert** apparaît avec un **chameau** apprivoisé à ses côtés (à 2 blocs de distance environ).

Reste dans/à côté d'un désert le temps qu'un marchand ambulant spawn (toutes les ~24 000 ticks par défaut, soit ~20 min). Approche le chameau et clic droit pour monter dessus → le succès se déclenche.

Le chameau t'appartient (pas besoin de le voler — il est déjà sans propriétaire).

## Éponge (via Grand Gardien)

Place un **gardien** dans une zone exposée au ciel pendant un orage. Frappe-le avec un **trident Canalisation** (ou amène un paratonnerre à proximité). Tous les gardiens dans un rayon de 12 blocs autour de la frappe sont convertis en **Grands Gardiens**.

Tue le Grand Gardien pour récupérer **1 éponge** (drop garanti pour la mort par joueur).

!!! tip "Multi-conversion"
    Tu peux convertir plusieurs gardiens d'un coup en les regroupant dans la zone d'effet.

## Piglin brute (spawn)

Pose des blocs dans la BB d'un **vestige de bastion** (ton Nether). Les piglins brutes spawnent dessus naturellement (weight 5, 1-2 par vague), en plus des piglins/hoglins/piglins zombifiés spawnés par biome.

## Éclat d'écho (via Warden sonic boom)

Force un **Warden** à frapper avec son **sonic boom** une **chauve-souris** ou un **dauphin** jusqu'à le tuer.

Si la dernière source de dégât du mob est le sonic boom du Warden, la victime drop **1 éclat d'écho** à sa mort.

!!! tip "Setup pratique"
    Amène un dauphin dans une rigole d'eau près d'un Warden et reste hors de portée le temps que le Warden charge son sonic boom (cooldown ~40 ticks).

## Hurleur sculk pré-placé

**1 hurleur sculk** est pré-placé à ~5 blocs du cadre en ardoise des abîmes renforcée de chaque ancienne cité. Idéal pour farm Warden (4 activations consécutives → spawn Warden).
