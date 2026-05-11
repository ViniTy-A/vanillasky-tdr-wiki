# Chambres des épreuves

Le système des **chambres des épreuves** sur TdR suit un modèle **strict CSA-Reborn** : pas d'activation passive, ressources rebalancées, et les ornements d'armure ne s'obtiennent **plus** via les coffres-forts mais via des challenges Tier 3.

## Générateur des épreuves activé via bâton de Breeze (STRICT)

**Le seul moyen d'activer un générateur des épreuves** est de cliquer-droit dessus avec un **bâton de Breeze** en main.

L'auto-activation par proximité de joueur (vanilla) est **désactivée** via le mixin `TrialSpawnerNoAutoActivateMixin` — le générateur reste éternellement `INACTIVE` tant que personne ne lui colle un bâton.

### Procédure complète

1. **Capture un Blaze** dans le Nether (ils spawnent dans la BB de forteresse)
2. Traverse le portail vers l'Overworld → **conversion en Breeze** (voir [Blaze → Breeze](mobs.md#blaze-breeze-passage-nether-overworld))
3. **Tue le Breeze** pour récupérer ≥1 **bâton de Breeze**
4. Trouve une **chambre des épreuves**, clic-droit sur un générateur des épreuves inactif avec ton bâton → activation forcée

Le combat démarre, vainc tous les mobs pour obtenir une **clé des épreuves** qui ouvre les coffres-forts rebalanced. **Consomme 1 bâton par activation**.

!!! info "Variant funeste"
    Les générateurs funestes (ominous) fonctionnent pareil — clic-droit avec un bâton de Breeze pour les activer.

## Loot des coffres-forts rebalancé (CSA-Reborn style)

Les loot tables des coffres-forts de chambre des épreuves ont été rebalancées pour ne plus être trivialisantes (basé sur CSA-Reborn).

### Coffre-fort régulier (clé des épreuves classique)

**Contient** :
- Motif de bannière rafaleur
- Les 3 tessons rares : **tourbillon / rafaleur / hache**

**Retiré** : pomme d'or, disque musical Precipice, trident, hache en diamant, plastron en diamant, Ornement des boulons.

### Coffre-fort funeste (clé des épreuves funeste)

**Contient** :
- Motif de bannière tourbillon
- Noyau lourd

**Retiré** : pomme d'or enchantée, disque musical Creator, disque musical Creator (Music Box), pomme d'or, blocs de diamant, Ornement des tourbillons.

### Disques de chambre des épreuves

Les 3 disques de chambre des épreuves (Creator, Creator Music Box, Precipice) sont **exclusivement via creeper-kill par squelette** dans la BB d'une chambre des épreuves — pas de double mécanique. Voir [Disques musicaux](disques.md).

### Ornements d'armure → Challenges Tier 3

Les **Ornements des boulons** et **Ornements des tourbillons** sont désormais récompenses des challenges :

- [Conquérant de la foudre](#conquerant-de-la-foudre-lightning-conqueror) (Tier 3)
- [Maîtrise du flux](#maitrise-du-flux-harnessing-the-flow) (Tier 3)

Comme dans CSA-Reborn original. Les loots commodity (émeraudes, fer, livres enchantés) restent dans `reward_rare`/`reward_ominous_rare`.

## Conquérant de la foudre (Lightning Conqueror)

Succès **Tier 3** — récompense : **Ornement des boulons** (`bolt_armor_trim_smithing_template`).

### Procédure

Foudroie **5 mobs spécifiques** avec un **trident enchanté Canalisation** pendant un orage :

- Creeper
- Gardien
- Mooshroom
- Piglin zombifié
- Sorcière

Chaque kill compte une seule fois — il faut donc varier les cibles.

Le trident Canalisation s'obtient en pêchant des noyés à trident (drop) puis enchant via table d'enchant ou livres.

## Maîtrise du flux (Harnessing the Flow)

Succès **Tier 3** — récompense : **Ornement des tourbillons** (`flow_armor_trim_smithing_template`).

### Procédure

Tiens un **trident enchanté Impulsion** en main avec l'effet **Pouvoir du conduit** actif sur toi.

L'effet vient d'un **conduit construit** :
- 8 coquilles de nautile
- 1 cœur de la mer
- Cadre de prismarine immergé

Le trident Impulsion est obtenable via noyé drop + enchant.

Le succès se débloque dès que tu remplis ces conditions simultanément (1 tick suffit).

## Succès de progression liés

| Succès | Trigger | Quand débloqué |
|---|---|---|
| `breeze_rod` | Inventory check | Avoir un bâton de Breeze dans l'inventaire |
| `activate_trial_spawner` | **Strict (clic réussi)** | Activer un générateur via bâton de Breeze |
| `music_disc_trial_chamber` | Inventory check ×2 | Avoir les disques Precipice + Creator |

Voir [Succès de progression](../roadmap.md) pour l'arbre complet.
