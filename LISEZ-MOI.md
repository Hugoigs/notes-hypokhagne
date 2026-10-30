# Mettre mon site de notes en ligne

Ce dossier est un site **Quartz** (le même outil que lenowe.github.io/notes-nowe-bl), déjà rempli avec mes notes `Hypokhagne`.

- `content/` : mes notes (copie du dossier Hypokhagne) + `content/attachments/` (les images, compressées)
- `content/index.md` : la page d'accueil (modifiable)
- `quartz.config.ts` : titre du site, couleurs, polices

## Mise en ligne (une seule fois, ~10 min)

1. Crée un compte sur https://github.com (gratuit).
2. Installe **GitHub Desktop** : https://desktop.github.com, connecte-toi avec ton compte.
3. Dans GitHub Desktop : *File → Add Local Repository…* → choisis ce dossier `notes-hypokhagne`. GitHub Desktop dit que ce n'est pas encore un dépôt : clique **create a repository**, puis **Create repository** (branche `main`).
4. Clique **Publish repository**. Décoche « Keep this code private » (GitHub Pages gratuit exige un dépôt public). Nom : `notes-hypokhagne`.
5. Sur github.com, ouvre ton dépôt → **Settings → Pages** → *Source* : **GitHub Actions**.
6. Onglet **Actions** → « Publier le site sur GitHub Pages » → **Run workflow**.
7. Après 2–3 min, le site est en ligne à : https://hugoigs.github.io/notes-hypokhagne/

(Le `baseUrl` est déjà réglé sur `hugoigs.github.io/notes-hypokhagne` : garde bien le nom de dépôt `notes-hypokhagne`.)

## Mettre à jour le site

Remplace le contenu de `content/` par la nouvelle version de tes notes, puis dans GitHub Desktop : écris un résumé → **Commit to main** → **Push origin**. Le site se reconstruit tout seul.
