# Voyages dimensionnels

## Portail du Nether

Construis un portail du Nether classique (4×5 obsidienne minimum, briquet pour l'allumer). À la première traversée, le serveur génère automatiquement le portail correspondant **dans ton Nether privé**, avec une **plateforme de 8 blocs** pour t'éviter de tomber dans le vide :

```
    A N N A
    N O O N
    O O O O    ← portail (rangée du bas)
    N O O N
    A N N A
```

*A = air · N = matériau de plateforme · O = obsidienne du portail (vue du dessus, même Y que la rangée d'obsidienne du bas)*

### Matériau de la plateforme

Le matériau **N** dépend du biome côté Nether :

| Biome Nether | Matériau |
|---|---|
| Forêt carmin | Nylium carmin |
| Forêt biscornue | Nylium biscornu |
| Terres désolées du Nether, Vallée de sable des âmes, Deltas de basalte | Netherrack |

### Côté retour

Du Nether vers ton Overworld, un nouveau portail créé reçoit aussi 8 blocs de **netherrack** en plateforme. La plateforme se génère **uniquement à la création du portail**, pas à chaque traversée.

## Portail de l'End

Trouve ton **fort** (stronghold, visible avec Mini-HUD ou repérable sur [chunkbase.net](https://www.chunkbase.net)), remplis l'anneau de cadres de portail de l'End avec **12 yeux de l'Ender** (à crafter vanilla : poudre de Blaze + perle de l'Ender), et saute.

Tu atterris sur la **plateforme d'obsidienne de spawn** dans **ton End**, avec ton dragon à toi.

### Portail de sortie

Le **portail de sortie** (au centre, à Y=60, après avoir tué le dragon) te ramène dans ton Overworld :

- Si tu as un **lit** dans ton Overworld → tu reviens à ton lit
- Sinon → tu reviens à **(0.5, 101, -2.5)**, ton île de départ

### Portails de l'End (gateways)

Quand tu utilises un **portail de l'End** (les petits portails bleus qui te tp d'un bord à l'autre du End), tu atterris sur une petite île de **pierre de l'End** générée à la volée.

!!! tip "Mécanique custom"
    **Sur chaque île de destination, une plante de chorus est plantée automatiquement.** Casse la fleur de chorus au sommet pour récupérer des fruits de chorus + des nouvelles fleurs. Renouvelable : chaque nouveau portail utilisé pour la première fois génère sa propre île + plante.
