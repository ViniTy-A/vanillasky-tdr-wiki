# Tuto — Descendre à Y=-64

En skyblock il n'y a **rien** sous ton île — juste le vide. Pour profiter des avantages des couches profondes (spawn rate boost, pas de phantoms), il faut **construire ta propre voie de descente bloc par bloc**. **Une seule technique est viable en early game** : la descente par trappes.

!!! info "Vidéo à venir"
    Tuto vidéo en cours d'enregistrement par l'admin du serveur.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Descente à Y=-64 par trappes — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen></iframe>
-->

## Pourquoi descendre ?

- **Taux de spawn de mobs plus élevé** — l'algorithme de spawn de MC choisit une Y aléatoire entre le bloc le plus haut de la colonne et Y=-64. Plus tu es bas, plus la plage est petite et concentrée sur ta plateforme
- **Pas de phantoms** — sous Y=64, l'absence d'accès direct au ciel empêche les phantoms de spawner au-dessus de toi

## Matériel requis

- **3 trappes** (n'importe quel bois — chêne suffit). Tu les récupères et tu les replaces à chaque step
- **~130 blocs** (pierre, terre, n'importe quoi de solide pour les placements vers le bas, 1 par bloc de descente)

## La technique — Descente par trappes

Le principe exploite le mode **allongé** (prone) qu'on prend automatiquement quand on est coincé sous une trappe fermée dans un espace d'1 bloc de haut. Allongé, ta reach permet de placer un bloc **1 bloc plus bas** que ta position, en visant une trappe voisine.

### Setup initial

1. **Trappe A** : place une trappe **dans le vide**, attachée sur le **bas d'un bloc** de ta plateforme (la trappe pend vers le vide)
2. **Trappe B** : fais **shift+clic-droit sur la Trappe A** avec une trappe en main → ça pose une 2e trappe **par-dessus** la première
3. **Trappe C** : pose une trappe sur **le dessus d'un autre bloc** voisin, en ayant **le vide en dessous** de cette trappe

### Procédure de descente (à répéter)

1. Mets-toi **sur la Trappe A** avec la **Trappe B ouverte** au-dessus
2. **Ferme la Trappe B** → tu te retrouves **allongé** (prone)
3. **Vise le DESSOUS de la Trappe C** et fais **shift+clic dessus avec un BLOC** en main → le bloc se pose **1 bloc plus bas** que la trappe ciblée
4. Tu as maintenant un nouveau « step » 1 bloc plus bas. Replace ta Trappe A / Trappe B / Trappe C autour de ce nouveau bloc et recommence

### Boucle de descente

À chaque itération, tu descends d'**1 bloc**. Pour aller de Y=64 à Y=-64, compte environ **128 itérations** soit **10-15 min** de descente.

!!! tip "Astuce"
    Garde toujours **plusieurs piles** dans ton hotbar : trappes en main 1, blocs en main 2. Switch rapide entre les deux pour optimiser le rythme.

!!! warning "Concentration"
    Si tu rates un shift+clic et que tu casses ta trappe support, tu **tombes** dans le vide jusqu'à la mort à Y=-64. Avance prudemment !

## Élytres (endgame seulement)

Une fois que tu as les **élytres** (via [Mécanique : Élytres](../mecaniques/mobs.md#elytres-via-endermite)), tu n'as plus besoin de cette technique : tu plane jusqu'en bas et tu stall horizontal au dernier moment.

Mais avant les élytres, la descente par trappes reste **la seule méthode early-game viable**.

## Astuces post-descente

Une fois arrivé à Y=-64 :

- **Construis ton spawn pad** — plateforme 16×16, light 0, drop chute de 24 blocs pour kill 1-shot (voir [Ferme à mobs sans eau](ferme-mobs-sans-eau.md))
- **Garde un retour** — construis un escalier ou ascenseur pour remonter facilement
- **Bedrock break/duping** ❌ — bug exploit non autorisé sur TdR, pas la peine d'essayer

## Liens connexes

- [Ferme à mobs sans water stream](ferme-mobs-sans-eau.md) — ce que tu construis une fois en bas
- [Setup client (Mini-HUD)](../setup-client.md) — pour voir les BB de structures profondes (ancienne cité notamment)
