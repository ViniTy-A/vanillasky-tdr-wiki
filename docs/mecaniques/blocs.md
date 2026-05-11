# Mécaniques blocs

## Sable

**Bloc / gorgone / plante de corail mort** adjacent à de l'eau (source ou courante) → **10%/scan tick (5s)** de chance d'éroder → devient eau + drop sable.

Compatible farms AFK (chunks force-loaded + `/island keepalive on`).

## Sable rouge

Même mécanique mais sur **corail de feu mort**. Drop **sable rouge** au lieu de sable.

## Diamant (renouvelable)

Pose un **bloc de charbon** au sol, fais tomber une **enclume** dessus (bloc qui chute). Le bloc de charbon disparaît et drop **1 diamant**. L'enclume continue sa chute.

!!! tip "Farm passif"
    Construis une tour à enclumes au-dessus d'une rangée de blocs de charbon. Chaque enclume qui tombe consomme 1 bloc et drop 1 diamant.

## Mycélium

Fait pousser un **énorme champignon** (poudre d'os sur un petit champignon rouge/brun). **Au moment de la pousse**, 2-4 blocs herbe/terre/podzol autour deviennent **mycélium** instantanément (comme du podzol sous les sapins).

## Buisson mort

Place une **pousse d'arbre** sur du **sable** (sable ou sable rouge). La pousse survit mais meurt lentement via random ticks → devient **buisson mort**.

## Buisson

Le nouveau bloc **buisson** de MC 1.21.x se génère uniquement dans certains biomes secs (badlands, désert) en worldgen, donc inaccessible dans les dimensions voidées.

**Mécanisme custom** :
1. Plante une pousse sur du sable → elle meurt en buisson mort (mécanique CSA existante)
2. Clic-droit sur le buisson mort avec une **fiole d'eau** → il devient un **buisson**

La fiole est consommée et une **fiole** vide est rendue.

Renouvelable infiniment via les pousses + sable + fioles d'eau.

## Blocs de corail (renouvelable)

Place **1 bloc d'algues séchées** entouré de **4+ blocs de corail du même type** (vivant ou mort) dans un 5×5×5. Les algues séchées se convertissent en ce corail.

| Biome | Vitesse de conversion |
|---|---|
| Biomes chauds / plaines | ~22 s |
| Biomes froids | ~40 s |
| Désert | jusqu'à 16 min |

**Source initiale des coraux** : marchand ambulant vanilla (8 blocs/troc).

## Druse d'améthyste

Mécanique CSA : reproduis manuellement le pattern d'une géode vanilla pour faire apparaître une druse d'améthyste.

1. Construis un cube **3×3×3 entièrement en basalte lisse**
2. Remplace le bloc du milieu par une source de **lave**
3. Remplace les 6 blocs **en contact direct avec la lave** (les faces — pas les arêtes ni les coins) par de la **calcite**

C'est exactement la structure d'une géode vanilla.

Toutes les **~2h** en moyenne, la lave se transforme en **druse d'améthyste**.

[:material-video: Voir le tutoriel visuel](../tutoriels/druse-amethyste.md){ .md-button }

## Pétales roses (via feuilles de cerisier)

Recette de four custom **uniquement pour les feuilles de cerisier** :

1. Récupère une **pousse de cerisier** via le marchand ambulant (trade tier 2)
2. Plante-la, applique de la **poudre d'os** pour faire pousser le cerisier
3. Casse les **feuilles de cerisier** avec des **cisailles** (ou un outil **Toucher de soie**) pour récupérer le bloc en item — sans cisailles tu n'auras que pommes/pousses/bâtons
4. Mets le bloc au four (10 s, 0.1 XP) → sortie : **1 pétale rose**

!!! warning "Spécifique aux cerisiers"
    Les autres feuilles fondues donnent toujours du **Tas de feuilles** (vanilla, recette inchangée). Seules les feuilles de cerisier produisent des pétales roses.

!!! tip "Source de teinture rose"
    Comme les pétales sont la seule source de teinture rose à coût 1 (vs peony 2 fleurs ou tulipe rose 1 fleur mais difficile à farm), c'est aussi la voie la plus efficace pour **teinture rose** (`1 pétale → 1 teinture` via crafting).

## Fruit / Fleur de chorus

Quand tu utilises un **portail de l'End** (les petits portails bleus qui te tp d'un bord à l'autre du End), tu atterris sur une petite île de **pierre de l'End** générée à la volée.

**Sur chaque île de destination, une plante de chorus est plantée automatiquement.** Casse la fleur de chorus au sommet pour récupérer des fruits de chorus + des nouvelles fleurs.

Renouvelable : chaque nouveau portail utilisé pour la première fois génère sa propre île + plante.

## Hautes herbes et Grande fougère (via enderman)

Le tag `enderman_holdable` est étendu pour inclure **hautes herbes** et **grande fougère**. Conséquence : un enderman peut ramasser ces blocs s'il en croise (la nuit, dans des zones avec de l'herbe).

Quand il tient un de ces blocs et qu'il est tué par le joueur, il drop le bloc en item (loot table custom).

C'est la **seule façon** d'obtenir ces 2 plantes hautes en survie — vanilla ne les drop pas autrement et elles ne sont pas craftables.

## Cœur de grinceur

Mécanisme de pousse custom dans le biome **jardin pâle** (pale_garden).

**Procédure** :
1. Trouve un biome jardin pâle (`chunkbase` + `/myseed`)
2. Récupère ≥4 pousses de chêne pâle via le marchand ambulant
3. Plante les 4 pousses dans un rayon de 4 blocs autour d'une **Œilchidée**
4. Quand l'une des 4 pousses grandit naturellement, elle a **10% de chance** de générer son arbre avec un **cœur de grinceur** intégré au sommet du tronc

Le cœur ainsi obtenu, place-le ailleurs adjacent à ≥2 bûches de chêne pâle pour qu'il invoque un **Grinceur** la nuit.

Mécanique 100% renouvelable — chaque pose de 4 pousses + Œilchidée donne en moyenne ~10 essais avant de proc.

## Lichen luminescent (via foudre)

Fais grimper des **lianes** contre un bloc de **pierre lumineuse**. Pendant un orage, frappe la pierre lumineuse avec un **trident enchanté Canalisation** (ou utilise un paratonnerre adjacent).

Toutes les lianes des 6 faces de la pierre lumineuse sont converties en **lichen luminescent** au moment de la frappe.

Récolte avec des cisailles.

## Terre des âmes (via feu de camp des âmes)

Récupère du **sable des âmes** via le troc des piglins (poids 5/459, ~1% par lingot d'or troqué). Crafte un **feu de camp des âmes** (4 bûches + 1 charbon ou charbon de bois + sable des âmes au centre).

Place-le **directement sur** un bloc de sable des âmes, puis casse-le. Le sable des âmes situé sous le feu de camp se convertit en **terre des âmes**.

Cycle renouvelable tant que tu peux farm du sable des âmes via les piglins.

## Fleur sporifère (via feuille d'azalée fleurie)

Casse une **feuille d'azalée fleurie** à mains nues ou avec un outil non-cisailles / non-toucher de soie.

| Niveau Fortune | Probabilité |
|---|---|
| F0 | 1.25% |
| F1 | 1.67% |
| F2 | 2.08% |
| F3 | 2.50% |

Avec une pioche **Fortune III**, en moyenne **1 fleur sporifère toutes les ~40 feuilles cassées**.

## Verrue du Nether (renouvelable, via chèvre)

Voir [Mécaniques mobs → Verrue du Nether](mobs.md#verrue-du-nether-renouvelable-via-chevre).
