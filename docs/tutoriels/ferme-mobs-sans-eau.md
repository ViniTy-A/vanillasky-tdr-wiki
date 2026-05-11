# Tuto — Ferme à mobs sans water stream

!!! warning "Page à écrire"
    Cette page sera rédigée par l'admin du serveur. La technique exacte (tour à mobs pathfind sans eau) sera expliquée ici avec vidéo à l'appui.

## Pourquoi sans eau

En skyblock TdR, l'eau n'est pas dispo en early game (voir [Premier seau d'eau](premier-seau-eau.md)). Les fermes à mobs vanilla utilisent très souvent de l'eau pour faire tomber les ennemies à l'endroit de kills. Il faut donc une alternative basée sur le **pathfinding** des mobs.

## Technique : tour à mobs pathfind

 Etant donné que l'on ne peut pas jouer sur l'eau pour faire tomber les mobs il va falloir jouer avec leurs IA.
 Pour ca on va utiliser un combo de de dalle / escalier ainsi que quelques blocs.
 Le but est que le mob spawn sur une dalle haute entouré d'escaliers, son objectif sera de rejoindre les blocs pleins à l'opposé de sa plateforme de spawn car un mob veut toujours être sur des blocs pleins et son IA finira toujours pas le pousser a y aller, des trappes lui feront croire qu'il pourra y acceder et il finira par tomber dans notre zone de kill.
 
*À compléter par l'admin avec procédure exacte + vidéo.*

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Ferme à mobs sans eau — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen></iframe>
-->

## Liens connexes

- [Premier seau d'eau](premier-seau-eau.md) — pourquoi tu as besoin de cette ferme dès le début
- [Descente à Y=-64](descente-y-64.md) — où placer ta ferme pour optimiser le spawn rate
