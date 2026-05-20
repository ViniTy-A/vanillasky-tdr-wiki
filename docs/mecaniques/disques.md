# Disques musicaux

Tous les disques musicaux exclusifs s'obtiennent via une mécanique custom : **un squelette tue un creeper dans la boîte englobante (BB) d'une structure spécifique**.

## Tableau des sources

| Disque | Structure (BB) | Poids dans le pool |
|---|---|---|
| Pigstep | Vestiges de bastion (Nether) | 3 (~20%) |
| Otherside | Fort / stronghold (Overworld) | 3 (~20%) |
| 11 | Manoir / woodland mansion | 3 (~20%) |
| Fragment de disque 5 | Ancienne cité | 18 (~60%) |
| Creator | Chambre des épreuves | 3 (~14%) |
| Creator (Music Box) | Chambre des épreuves | 3 (~14%) |
| Precipice | Chambre des épreuves | 3 (~14%) |

## Disques musicaux Pigstep / Otherside / 11

Squelette tue un creeper dans la **BB de la structure correspondante**. Pondéré weight 3 dans le pool — environ **20% de chance** qu'un creeper-kill dans la BB drop le disque.

## Fragment de disque 5

Squelette tue un creeper dans la **BB d'une ancienne cité**. Pondéré **weight 18** (~60% si dans la BB).

Combine **9 fragments** dans une table de craft pour obtenir le **disque musical 5**.

## Disques Creator / Creator (Music Box) / Precipice

Les **3 disques exclusifs aux chambres des épreuves** tombent quand un squelette tue un creeper dans la **BB d'une chambre des épreuves** (`trial_chambers`).

Chacun pondéré **weight 3** dans le pool — ensemble, **~43% de chance** qu'un creeper-kill dans la BB drop un de ces 3 disques.

!!! info "Source unique"
    Pas de mécanique double. Les 3 disques ne sont plus dans le coffre-fort funeste — uniquement via creeper-kill par squelette.

## Tessons de poterie

### Tessons de tourbillon / rafaleur / hache

Les tessons de poterie de **tourbillon**, **rafaleur** et **hache** apparaissent dans le butin des **coffres-forts uniques** des chambres des épreuves (poids 2/16 → **~12% par tirage**).

### Les 23 tessons vanilla sont accessibles

Combinés aux 20 autres tessons obtenables via le **renifleur** et l'**archéologie**, les **23 tessons vanilla** sont tous accessibles dans TdR.

## Setup pour farm creeper-via-squelette

Pour faciliter l'obtention de ces disques :

1. Identifie la BB de la structure (Mini-HUD + chunkbase pour les positions)
2. Construis une zone d'arène **à l'intérieur de la BB** (au moins quelques chunks)
3. Configure des spawns squelette + creeper proche
4. Le squelette doit tirer une flèche sur le creeper pour le tuer

!!! tip "AFK farm"
    Reste à proximité (dans la simulation distance) pour que les chunks tickent et que les mobs spawnent.
