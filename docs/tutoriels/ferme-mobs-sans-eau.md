# Tuto — Ferme à mobs sans eau

## Pourquoi sans eau

En skyblock TdR, l'eau n'est pas dispo en early game (voir [Premier seau d'eau](premier-seau-eau.md)). Les fermes à mobs vanilla utilisent très souvent de l'eau pour faire tomber les mobs à l'endroit de kills. Il faut donc une alternative basée sur le **pathfinding** des mobs.

## Technique : tour à mobs pathfind

Étant donné que l'on ne peut pas jouer sur l'eau pour faire tomber les mobs, il va falloir jouer avec leur IA. Pour ça on utilise un combo de dalles / escaliers ainsi que quelques blocs.

Le but est que le mob spawn sur une dalle haute entourée d'escaliers. Son objectif sera de rejoindre les blocs pleins à l'opposé de sa plateforme de spawn (un mob veut toujours être sur des blocs pleins), et son IA finira toujours par le pousser à y aller. Des trappes lui font croire qu'il peut y accéder et il finit par tomber dans ta zone de kill.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Ferme à mobs sans eau — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen></iframe>
-->

## Variantes — 3 tailles selon ton niveau de farm

Plus la tour est large, plus elle spawn de mobs en parallèle. Choisis selon les bûches que tu as et le débit que tu veux atteindre.

<div class="grid cards" markdown>

-   :material-numeric-1-circle:{ .lg .middle } **Tour simple**

    ---

    Compacte, parfaite pour démarrer dès que tu as descendu à Y=-64.

    **~229 bûches de chêne · ≈3,6 stacks**

    | Matériau | Quantité |
    |---|---:|
    | Planches de chêne | 200 |
    | Dalle en chêne | 344 |
    | Escalier en chêne | 300 |
    | Trappe en chêne | 30 |

    [:material-download: Télécharger .litematic](../assets/schematics/tour-mob-simple.litematic){ .md-button .md-button--primary }

-   :material-numeric-2-circle:{ .lg .middle } **Tour double**

    ---

    2× plus de plateformes de spawn pour un footprint contenu.

    **~334 bûches de chêne · ≈5,2 stacks**

    | Matériau | Quantité |
    |---|---:|
    | Planches de chêne | 320 |
    | Dalle en chêne | 440 |
    | Escalier en chêne | 426 |
    | Trappe en chêne | 50 |

    [:material-download: Télécharger .litematic](../assets/schematics/tour-mob-double.litematic){ .md-button .md-button--primary }

-   :material-numeric-4-circle:{ .lg .middle } **Tour quad**

    ---

    Le format endgame — débit ~4× la tour simple.

    **~580 bûches de chêne · ≈9,1 stacks**

    | Matériau | Quantité |
    |---|---:|
    | Planches de chêne | 320 |
    | Dalle en chêne | 840 |
    | Escalier en chêne | 852 |
    | Trappe en chêne | 99 |

    [:material-download: Télécharger .litematic](../assets/schematics/tour-mob-quad.litematic){ .md-button .md-button--primary }

</div>

## :material-pine-tree: Récap bûches de chêne par tour

| Tour | Bûches nécessaires | Stacks |
|---|---:|---:|
| **Tour simple** | 229 bûches | ~3,6 stacks |
| **Tour double** | 334 bûches | ~5,2 stacks |
| **Tour quad** | 580 bûches | ~9,1 stacks |

!!! info "Comptage du bois"
    Le nombre de bûches inclut le craft de tous les sous-produits (planches → dalles, escaliers, trappes). Garde un peu de marge pour les erreurs de pose : prévoir +5% est une bonne habitude.

## Comment utiliser les schematics

1. Installe **[Litematica](https://modrinth.com/mod/litematica)** côté client (mod Fabric 1.21.11)
2. Télécharge le `.litematic` de ton choix avec un des boutons ci-dessus
3. Place le fichier dans `<dossier-minecraft>/schematics/` (ou clique-droit → **Enregistrer la cible sous** directement dans ce dossier)
4. En jeu : `M` pour ouvrir le menu Litematica → **Schematic Browser** → ouvre ton fichier → **Load schematic**
5. Le hologramme apparaît à ta position. Pose les blocs en suivant le hologramme bloc par bloc

!!! tip "Liste matérielle visuelle"
    Dans Litematica, ouvre la **Material List** (raccourci par défaut `H` ou via le menu `M`) pour voir en temps réel les blocs manquants par rapport à la sélection. Pratique pour savoir exactement combien il te reste à crafter avant de commencer.

!!! warning "Toujours light-proof"
    Place ta tour **à Y=-64** ou au moins très bas dans le deepslate, et **light-proof toute zone autour** (light level 0 partout sauf dans la tour). Sinon les mobs spawn ailleurs et ton taux de drop chute.

## Liens connexes

- [Premier seau d'eau](premier-seau-eau.md) — pourquoi tu as besoin de cette ferme dès le début
- [Descente à Y=-64](descente-y-64.md) — où placer ta ferme pour optimiser le spawn rate
- [Setup client](../setup-client.md) — installer Litematica et les autres mods clients recommandés
