# Vanilla Sky TdR — Wiki

Manuel du joueur du serveur Skyblock **Vanilla Sky TdR** (« Tout de Rien ») — Fabric MC 1.21.11.

🌐 **Site publié** : https://vinity-a.github.io/vanillasky-tdr-wiki/

## Structure

```
wiki/
├── mkdocs.yml              ← config MkDocs Material (thème, nav, plugins)
├── requirements.txt        ← deps Python (mkdocs-material)
├── .github/workflows/
│   └── deploy.yml          ← build + deploy auto à chaque push sur main
└── docs/                   ← contenu du wiki en Markdown
    ├── index.md            ← page d'accueil
    ├── concept.md
    ├── voyages-dimensionnels.md
    ├── spawn.md
    ├── commandes.md
    ├── recettes/           ← recettes custom
    ├── mecaniques/         ← mécaniques de gameplay
    ├── tutoriels/          ← tutos vidéo YouTube
    └── ...
```

## Éditer

### Via l'éditeur web GitHub (le plus simple)

1. Va sur https://github.com/ViniTy-A/vanillasky-tdr-wiki
2. Navigue dans `docs/`, clique sur la page à modifier
3. Bouton crayon (Edit) → fais tes changements en Markdown
4. **Commit changes** → le site se rebuild automatiquement (~1 min)

### Via clone local (pour gros changements ou preview)

```bash
git clone https://github.com/ViniTy-A/vanillasky-tdr-wiki.git
cd vanillasky-tdr-wiki
pip install -r requirements.txt
mkdocs serve  # preview live sur http://127.0.0.1:8000
```

Édite les `.md` → le serveur dev recharge automatiquement.

Quand t'es content :
```bash
git add .
git commit -m "describe what you changed"
git push
```

→ Le site se rebuild + redéploie tout seul via GitHub Actions.

## Ajouter une vidéo tutoriel

1. Upload la vidéo sur YouTube en **Non répertorié** (visible uniquement avec le lien)
2. Récupère l'**ID de la vidéo** (la partie après `v=` dans l'URL, ex: `dQw4w9WgXcQ`)
3. Dans le `.md` de ton tuto, colle :

```markdown
<iframe
  width="100%"
  height="500"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Titre de la vidéo"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
```

Remplace `VIDEO_ID` par ton ID. C'est tout.

## Convention de noms vanilla FR

Tous les termes Minecraft doivent utiliser les noms **vanilla français Java** officiels (source : fr.minecraft.wiki). Quelques pièges à éviter :

| ✅ Correct | ❌ Faux |
|---|---|
| Breeze | Brise |
| Bâton de Breeze | Bâton de brise |
| Ender Dragon | Dragon de l'End |
| Mooshroom | Champimeuh |
| Coffre-fort funeste | Coffre-fort sinistre / Voûte |
| Clé des épreuves | Clé d'épreuve |
| Chambres des épreuves | Chambre d'épreuve |
| Générateur des épreuves | Générateur d'épreuve / Trial spawner |
| Fiole / Fiole d'eau | Bouteille / Bouteille d'eau |
| Hautes herbes | Herbe haute |
| Herbe aquatique | Algue (= kelp) |
| Araignée chevauchée | Cavalier d'araignée / Spider jockey |
| Ghast joyeux | Joyeux Ghast / Happy Ghast |
| Pomme de terre empoisonnée | Patate empoisonnée |
| Chèvre beuglante | Chèvre hurleuse / Chèvre hurlante |
| Vestiges de bastion | Vestige de bastion / Bastion remnant |
| Ornement des boulons | Modèle de forge — Boulon |
| Ornement des tourbillons | Modèle de forge — Tourbillon |
