# Tuto — Druse d'améthyste artificielle

Construis une géode artificielle qui produit une **druse d'améthyste** toutes les ~2h en moyenne. C'est la seule façon d'obtenir l'améthyste en skyblock.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 0.3rem; margin: 1.5rem 0; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
  <iframe
    src="https://www.youtube-nocookie.com/embed/hqDanaDjJGo?rel=0"
    title="Druse d'améthyste artificielle — Vanilla Sky TdR"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0;"
    loading="lazy"
    allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen></iframe>
</div>

<p style="text-align: center; margin-top: -0.5rem; font-size: 0.85em; opacity: 0.7;">
  <a href="https://youtu.be/hqDanaDjJGo" target="_blank" rel="noopener">▶ Regarder sur YouTube</a>
  · Le tuto écrit ci-dessous reprend les mêmes étapes en référence
</p>

## Matériel requis

- 20 blocs de **basalte lisse** (du basalte + 4 fonte au haut fourneau OU table de tailleur)
- 6 blocs de **calcite** (diorite cuite au haut fourneau — voir [recette](../recettes/haut-fourneau.md))
- 1 seau de **lave**

## Étape 1 — Cube de basalte lisse 3×3×3

Construis un cube **3×3×3 entièrement en basalte lisse** (27 blocs au total, dont 20 visibles + 1 caché au centre que tu remplaceras à l'étape 2).

## Étape 2 — Remplace le bloc central par de la lave

Le bloc du milieu du cube (celui caché à l'intérieur) → remplace-le par une **source de lave**.

## Étape 3 — Remplace les 6 faces par de la calcite

Remplace les **6 blocs en contact direct avec la lave** (les faces — pas les arêtes ni les coins) par de la **calcite**.

C'est exactement la structure d'une géode vanilla :

```
Vue du dessus (couche du milieu) :
. C .
C L C
. C .

Vue de côté (idem sur les autres axes) :
. C .
C L C
. C .
```

*C = calcite · L = lave · . = basalte lisse*

## Étape 4 — Attendre la conversion

Toutes les **~2h en moyenne**, la lave centrale se transforme en **druse d'améthyste**.

Pour accélérer : laisse les chunks chargés (`/island keepalive on`) et fais d'autres choses pendant ce temps.

## Étape 5 — Récolter

Casse une calcite pour accéder à la druse et commencer à récolter des **cristaux d'améthyste** qui poussent sur ses 6 faces.

!!! warning "Pas de propagation"
    Seul le pattern lave + calcite + basalte lisse produit une nouvelle druse d'améthyste. Les cristaux d'améthyste qui poussent dessus ne permettent pas d'en faire pousser ailleurs — pour chaque druse supplémentaire que tu veux, refais la mécanique depuis le début (lave centrale + 6 calcite + 20 basalte lisse).

## Astuces

- Récolte les cristaux avec une **pioche sans Toucher de soie** pour obtenir 4 éclats d'améthyste par cristal
- Une druse génère un cristal sur une face vide toutes les ~10 min en moyenne
- Avec 5+ druses en parallèle, tu sécurises un flow régulier d'éclats
