# Commandes

Toutes les commandes spécifiques au serveur TdR.

## `/myseed`

Affiche la seed de ton monde. **Clic-gauche sur le nombre** dans le chat pour la copier automatiquement dans ton presse-papiers, puis colle-la dans l'outil de ton choix (Chunkbase, Cubiomes Viewer, MineAtlas…) pour planifier tes explorations depuis le spawn.

La seed est **partagée entre tes 3 dimensions** (Overworld, Nether, End utilisent la même seed).

!!! tip "Alias FR"
    `/maseed` fait la même chose.

!!! warning "Adblock recommandé pour Chunkbase"
    Chunkbase est l'outil de référence mais sa régie pub laisse passer des **fausses alertes antivirus** ("Your computer is infected — Avast"). Installe **uBlock Origin** dans ton navigateur avant d'y aller. Voir [Setup client → Chunkbase](setup-client.md#chunkbase).

## `/island keepalive on|off`

Contrôle si tes 3 mondes restent chargés quand tu es déconnecté.

| Option | Comportement |
|---|---|
| `off` (défaut) | Tes mondes sont déchargés dès que tu quittes. Les farms AFK ne tournent plus. |
| `on` | Tes 3 mondes (Overworld + Nether + End) restent chargés. Tes farms AFK continuent, tes plantes poussent. |

!!! warning "Coût ressources"
    `keepalive on` fait tourner ton serveur même quand tu ne joues pas. À utiliser avec parcimonie (le serveur consomme des ressources pour toi).

## `/recompense`

Délivre les récompenses en attente quand ton inventaire était plein lors de l'obtention d'un succès. Si l'inventaire est encore plein, te dit combien restent en attente.

## `/reset` · alias FR `/recommencer`

**Reset complet de ton île** en cas de softlock RNG (notamment quand ton chêne de spawn n'a rien drop comme pousse — environ 1 chance sur 20).

### Procédure en deux temps

1. Tape `/reset` → un avertissement détaille ce qui va être effacé (3 dimensions, inventaire, succès Vanilla Sky)
2. Dans les **30 secondes**, confirme avec `/reset confirm` (ou `/reset confirmer`)
3. Tu peux annuler la demande avec `/reset annuler` avant la confirmation

### Cooldown

**15 minutes** entre deux resets confirmés.

### Ce qui est réinitialisé

Une fois la confirmation passée, le serveur te déplace en zone d'attente, supprime tes 3 dimensions, vide ton inventaire/XP, révoque tes succès `vanillasky:*`, recrée fresh les dimensions avec une nouvelle seed, puis te téléporte sur la nouvelle île de spawn.

!!! info "Conservé"
    Les succès vanilla MC et tes recettes apprises ne sont **pas** réinitialisés (seuls les succès `vanillasky:*` le sont). C'est volontaire : ça permet de rebooter la run sans tout perdre côté UI.

## Commandes admin (OP)

Réservées aux opérateurs niveau 2+ (gestion serveur).

### `/god`

Toggle invulnérabilité totale. Restaure aussi la vie max + saturation au moment de l'activation.

### `/fly`

Toggle mode vol survie.

### `/heal`

Restaure pleine vie + saturation + éteint le feu.

### `/feed`

Restaure la barre de faim.
