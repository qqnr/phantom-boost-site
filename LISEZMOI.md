# Site Phantom Boost (GitHub Pages)

Site statique : `index.html` + dossier `assets/` + `favicon.png`. Rien à construire.

## Mettre en ligne
1. Sur GitHub (compte qqnr), crée un dépôt **public**, par exemple `phantom-boost-site`.
2. « Add file » → « Upload files » : glisse `index.html`, `favicon.png` et le dossier `assets`. « Commit changes ».
3. Settings → Pages → Source : **Deploy from a branch**, Branch : **main**, dossier **/ (root)**, Save.
   Le site est en ligne sur https://qqnr.github.io/phantom-boost-site/ après une minute.

## Ton nom de domaine
1. Settings → Pages → **Custom domain** : tape ton domaine, Save (avant de toucher au DNS).
2. Chez ton registrar, ajoute 4 enregistrements **A** pour le domaine principal :
   185.199.108.153 · 185.199.109.153 · 185.199.110.153 · 185.199.111.153
   et un **CNAME** `www` → `qqnr.github.io`
3. Quand le certificat est prêt, coche **Enforce HTTPS**.

## À modifier facilement
- Lien de téléchargement / dépôt : `const REPO = "qqnr/phantom-boost"` dans `index.html`.
- Version et nombre de téléchargements : lus en direct sur GitHub.
- Image d'aperçu (Discord, X…) : `assets/img/og.jpg`, déjà en adresse complète (phantomboost.xyz). Si tu changes de domaine, remplace
  `content="assets/img/og.jpg"` par l'adresse complète (`https://ton-domaine/assets/img/og.jpg`).
- Police Poppins : licence OFL dans `assets/fonts/LICENSE.txt`.
