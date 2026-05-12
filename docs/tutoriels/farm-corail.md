# Tuto — Farm de coraux automatique

Les **blocs de corail** sont la source du **sable** sur TdR (via érosion en contact avec l'eau). Construire un farm automatique te permet de générer du sable en illimité, et c'est aussi joli.

!!! info "Vidéo à venir"
    Enregistrement vidéo à venir.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Farm de coraux automatique" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
-->

## Pré-requis

- Avoir reçu **au moins 4 blocs de corail** du marchand ambulant (trade 8 blocs/troc)
- ≥1 **bloc d'algues séchées** (algues = kelp, séchées au four)
- Blocs pour construire la structure
- Quelques seaux d'eau

## Principe — Mécanique de propagation

Sur TdR, **1 bloc d'algues séchées** entouré de **4+ blocs de corail du même type** dans un 5×5×5 se convertit en ce corail.

La vitesse dépend de la **température du biome** : sweet spot autour de 0.65. Plus la température s'éloigne de cette valeur (dans un sens **ou** l'autre), plus la conversion est lente.

| Catégorie | Biomes concernés | Vitesse |
|---|---|---|
| **Tempéré** (temp 0.5-0.8) | Océan chaud, plaines, forêt, jungle | ~22-24 s |
| **Froid** (temp 0-0.4) | Taïga, océan glacé, neige | ~26-40 s |
| **Brûlant extrême** (temp 2.0) | Désert, badlands (toutes variantes) | ~16 min |

→ Place ta farm dans un **biome tempéré** (océan chaud, plaines, forêt) pour les meilleures vitesses. **Évite désert et badlands** — leur température extrême (2.0) clamp le suitability à 0 et ralentit énormément.

## Architecture — Cellule simple

### Layout 5×5×5

```
Vue du dessus, couche du milieu :

C C C C C
C . . . C
C . A . C
C . . . C
C C C C C

```

*C = bloc de corail (vivant ou mort, mais du MÊME type) · A = bloc d'algues séchées*

Tu as besoin d'au moins **4 coraux** du même type dans le 5×5×5. Le pattern montre 16 pour bien remplir le cube, mais 4 suffit.

### Multi-couches

Pour optimiser, fais un cube **5×5×5 entier** avec toutes les couches comme la couche du milieu. Tu places ton bloc d'algues séchées au centre, et chaque tick il a plus de chance de convertir.

## Automatisation

### Eau partout

Toute la cellule doit être **immergée** dans l'eau (sinon les coraux meurent au bout de quelques secondes).

Place une **source d'eau** au-dessus pour que ça remplit le cube par la gravité, OU place 4 sources aux coins puis remplis avec des seaux.

## Coraux disponibles

Le marchand ambulant vend les **5 variantes** de blocs de corail :

- 🟦 Corail tube (blue)
- 🟪 Corail cerveau (pink)
- 🟧 Corail à bulles (purple)
- 🟥 Corail de feu (red)
- 🟨 Corail à cornes (yellow)


## Du corail au sable

Voir [Mécanique : Sable](../mecaniques/blocs.md#sable) pour la conversion corail mort → sable.

En résumé :
1. Casse les blocs de corail vivants → ils meurent en quelques secondes
2. Les coraux morts adjacents à de l'eau ont 10%/scan tick (5s) de chance d'éroder
3. Ils deviennent eau et drop du sable

→ Le corail de feu mort donne du **sable rouge** au lieu du sable normal.

## Astuces

- **`/island keepalive on`** : laisse le farm tourner même offline pour accumuler du stock
- **Multi-biomes** : si possible, place tes différents farms de coraux dans différents biomes pour comparer les vitesses
- **Décoration** : les blocs de corail vivants sont magnifiques pour décorer ton base / l'extérieur

## Liens connexes

- [Mécanique : Sable (érosion corail)](../mecaniques/blocs.md#sable)
- [Mécanique : Blocs de corail renouvelable](../mecaniques/blocs.md#blocs-de-corail-renouvelable)
- [Marchand ambulant](../vocabulaire.md#marchand-ambulant-wandering-trader)
