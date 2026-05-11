# Tuto — Farm Warden (ancienne cité)

Le **Warden** est nécessaire pour obtenir l'**éclat d'écho** (via sonic boom sur chauve-souris/dauphin) et le **catalyseur sculk** (via propagation). Ce tuto montre comment le farmer en sécurité depuis l'ancienne cité préservée.

!!! info "Vidéo à venir"
    Enregistrement vidéo à venir.

<!--
<iframe width="100%" height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Farm Warden — Vanilla Sky TdR" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
-->

## Pré-requis

- Localisation d'une **ancienne cité** (`/myseed` + chunkbase.net)
- Armure complète **Netherite Protection IV** (le Warden one-shot tout en dessous)
- **Bouclier** de qualité
- Potions de **Régénération**, **Résistance**, **Vitesse**
- Lait (pour annuler les effets Darkness si besoin)
- Pioche en diamant/Netherite Toucher de soie (pour les catalyseurs sculk)

!!! danger "Tu peux mourir"
    Même avec full Netherite Prot IV, **un sonic boom du Warden peut te tuer si tu n'as pas de Résistance**. Préfère farm à distance/depuis un endroit safe.

## La préservation TdR

L'ancienne cité sur TdR conserve :
- Le **cadre central en ardoise des abîmes renforcée** (8×8 environ)
- **1 hurleur sculk** pré-placé à ~5 blocs avec `can_summon=true`

Les autres blocs (sculk, capteurs, etc.) ne sont **pas** préservés — tu dois les recréer toi-même pour la propagation, mais le hurleur central permet déjà de spawner le Warden.

## Étape 1 — Localiser et atteindre la cité

1. Coordonnées sur chunkbase
2. Construis un pont jusqu'au-dessus de la zone
3. Mine vers Y=-50 environ (les anciennes cités sont profondes)

Le cadre + hurleur sont au centre de la BB de la structure.

## Étape 2 — Construire une zone safe d'activation

Le hurleur active un Warden après **4 activations consécutives** (chacune par bruit du joueur — saut, casse-bloc, etc., dans un rayon de 16 blocs).

Pour farmer en sécurité :
1. Crée une **plateforme suspendue à 5 blocs au-dessus du hurleur** (le Warden ne saute pas haut)
2. Murs en obsidienne / blocs résistants à l'explosion
3. Une **fente d'1 bloc** pour tirer avec ton arc / lancer des tridents Canalisation

## Étape 3 — Spawner un Warden

Saute sur ta plateforme 4 fois pour activer le hurleur 4 fois (1 saut = 1 activation environ).

→ Le Warden spawn à proximité de l'hurleur.

!!! tip "Effet Darkness"
    Pendant que le hurleur s'active, tu reçois l'effet **Darkness**. Bois du **lait** pour l'annuler si ça te gêne (ou attends que ça passe seul).

## Étape 4 — Loot via Warden

### Pour Éclat d'écho

Place une **chauve-souris** ou un **dauphin** dans une rigole d'eau / cage à portée du Warden. Reste hors de la portée du sonic boom (~15 blocs). Le Warden charge son sonic boom (cooldown ~40 ticks) et le tire sur la créature.

→ Si le sonic boom est la **dernière source de dégât**, la créature drop **1 éclat d'écho**.

### Pour Catalyseur sculk

Amène plusieurs zombies/squelettes dans la zone du Warden. Chaque kill du Warden propage la **sculk** autour du cadavre via les particules d'XP.

Avec une chance, des **catalyseurs sculk** apparaissent dans la propagation. Mine-les avec **Toucher de soie** pour les récupérer.

### Pour Membrane de sculk (vanilla)

Tu peux aussi tuer le Warden directement — il drop 1 **catalyseur sculk** garanti à la mort. Mais c'est très dangereux (~600 PV, hits forts).

## Astuces

- **Pas de farm AFK** : le Warden disparaît après 60s sans cibler quelqu'un. Tu dois être présent et actif.
- **Plusieurs hurleurs** : tu peux placer des hurleurs additionnels que tu mines (Toucher de soie) ailleurs. Mais celui pré-placé suffit pour les premières fois.
- **Sculk catalyst propagation** : place des **points de spawn proches** (donjon, spawner zombie improvisé) pour que les cadavres se concentrent dans la zone du Warden.

## Liens connexes

- [Mécanique : Éclat d'écho](../mecaniques/mobs.md#eclat-decho-via-warden-sonic-boom)
- [Mécanique : Catalyseur sculk](../mecaniques/mobs.md#catalyseur-sculk-via-warden)
- [Hurleur sculk pré-placé](../mecaniques/drops.md#hurleur-sculk-can_summon-pre-place)
