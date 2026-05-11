# Tuto — Descendre à Y=-64 sans seau d'eau

Quand tu débutes sur ton île à Y=64, tu n'as pas tout de suite un seau d'eau pour faire un bucket-MLG en bas. Voici plusieurs techniques pour descendre en sécurité jusqu'à Y=-64 (128 blocs en dessous).

!!! info "Vidéo à venir"
    Le tuto vidéo sera ajouté ici dès qu'enregistré.

<!-- Bloc à remplir avec ton iframe YouTube une fois la vidéo prête :
<iframe
  width="100%"
  height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Descente à Y=-64 — Tuto Vanilla Sky TdR"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
-->

## Pourquoi descendre ?

- **Spawn rate de mobs ×2 ou plus** — plus tu es bas dans le monde, plus les mobs hostiles spawnent souvent et en plus grand nombre (la mob cap par chunk se charge davantage dans les couches profondes vu que tu y monopolises la zone de spawn)
- **Pas de phantoms** — sous Y=64, l'absence d'accès direct au ciel empêche les phantoms de spawner au-dessus de toi. Tu peux dormir tranquille sans set up de spleef anti-phantom
- **Light level 0 facile** — pas de soleil, pas de luminescence ambiante. Tes plateformes de spawn sont sombres par défaut sans torch management

## Technique 1 — Pilier de blocs (le plus simple)

1. Mets-toi en mode descente lente (shift)
2. Place un bloc sous tes pieds en regardant vers le bas
3. Avance d'un demi-bloc, place un autre bloc sous tes pieds
4. Répète jusqu'en bas

**Temps** : ~4 min de Y=64 à Y=-64.

**Inconvénient** : très chronophage si tu vas vraiment loin.

## Technique 2 — Chute contrôlée avec lit

1. Place un **lit** sur la surface où tu veux atterrir (besoin de 3 laine + 3 bois)
2. Saute du haut, la chute sur un lit annule **50% des dégâts de chute** *(faux pour TdR — clarification suit)*

!!! warning "Pas en survie ici"
    Cette technique fonctionne en Bedrock, mais en **Java Edition** un lit n'annule pas les dégâts de chute. **Ne pas utiliser** pour de grandes hauteurs.

## Technique 3 — Foin (hay bale)

Les **balles de foin** annulent **80% des dégâts de chute** quand tu atterris dessus.

Pour atterrir à Y=-64 depuis Y=64 = 128 blocs de chute = ~125 dégâts vanilla → avec 80% absorbés = ~25 dégâts. **Tu meurs encore**.

Solution : empile **2+ couches de balles de foin**. Au-delà de la première, l'effet se cumule de manière étrange en Java, mais souvent ça marche.

## Technique 4 — Effet Chute lente

Si tu as accès à des potions de **Chute lente** (drop possible des phantoms en zone ouverte) :

1. Bois ou applique une potion de Chute lente (durée 1m30s)
2. Tu tombes à vitesse réduite, **plus de dégâts de chute**
3. Saute du haut, atterris peinard

**Inconvénient** : nécessite d'avoir déjà du matériel.

## Technique 5 — Échafaudage

Les **échafaudages** (scaffolding) permettent de monter et descendre rapidement (touche shift en bas pour descendre 1 bloc à la fois).

Recette : 6 bambous + 1 ficelle → 6 échafaudages.

Le bambou se trouve dans les jungles ou via marchand ambulant (saplings vendus).

**Avantage** : très rapide à descendre/monter, peu cher en ressources.

## Technique 6 — Élytres (endgame)

Une fois que tu as les élytres ([via endermite](../mecaniques/mobs.md#elytres-via-endermite)), descendre est trivial : tu plane jusqu'en bas.

Pour atterrir sans dégâts : pique un peu vers le sol au dernier moment puis stall horizontal pour ralentir.

## Technique recommandée selon ton stade

| Stade | Technique recommandée |
|---|---|
| Tout début (rien que pousses + chêne) | Pilier de blocs |
| Bambou récupéré | Échafaudage |
| Élevage + bois | Pilier ou échafaudage |
| Mid-game (potions, phantoms farmables) | Potion de Chute lente |
| Endgame | Élytres |
