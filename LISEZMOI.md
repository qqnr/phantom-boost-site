# Site Phantom Boost (GitHub Pages)

Site statique : `index.html` + dossier `assets/` + `favicon.png` + `CNAME`. Rien à construire.

## Mettre le site à jour
1. Sur GitHub, ouvre ton dépôt du site (par exemple `qqnr/phantom-boost-site`).
2. Supprime l'ancien dossier `assets` : ouvre-le → les trois points en haut à droite → **Delete directory** → Commit.
3. **Add file → Upload files** : glisse `index.html`, `favicon.png`, `CNAME`, `LISEZMOI.md` et le dossier `assets`.
   « Commit changes ». Les fichiers du même nom sont remplacés.
4. Une à deux minutes plus tard, phantomboost.xyz affiche la nouvelle version (Ctrl+F5 pour forcer le rechargement).

## Automatique
- Bouton Download : toujours la dernière release (`PhantomBoost-Setup.exe`) de `qqnr/phantom-boost`.
- Numéro de version du bouton final et nombre de téléchargements : lus en direct sur GitHub.
- Le texte « v1.0.18 » du bandeau NEW et de la section « Update » est écrit à la main : change-le à la prochaine grosse mise à jour.

## À modifier facilement
- Dépôt de l'appli : `const REPO = "qqnr/phantom-boost"` dans `index.html`.
- Captures de l'appli : `assets/img/app/*.webp` (1600 px de large).
- Image d'aperçu (Discord, X…) : `assets/img/og.jpg` (1200 × 630).
- Police Poppins : licence OFL dans `assets/fonts/LICENSE.txt`.
