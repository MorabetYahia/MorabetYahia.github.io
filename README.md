# Portfolio — Yahia Morabet

Site statique (HTML/CSS/JS, aucune dépendance à installer).

## Lancer en local
- Le plus simple : double-clic sur `index.html`.
- Ou, depuis ce dossier : `python -m http.server 8000` puis ouvrir http://localhost:8000
- Ou l'extension VS Code « Live Server » : clic droit sur index.html → Open with Live Server.

## Mettre en ligne gratuitement (GitHub Pages)
1. Créer un dépôt public nommé exactement `MorabetYahia.github.io`.
2. Y pousser le contenu de ce dossier (index.html à la racine + dossier assets/).
   ```
   git init && git add . && git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/MorabetYahia/MorabetYahia.github.io.git
   git push -u origin main
   ```
3. Settings → Pages → Source : « Deploy from a branch » → main / (root).
4. Le site est en ligne sur https://morabetyahia.github.io (1 à 2 minutes).

## Ajouter les vraies animations de l'avatar
Placer les frames dans `assets/frames/<etat>/001.webp, 002.webp…` puis remplir
l'objet `STATES` dans le script de index.html. Ajouter `#debug` à l'URL pour voir les zones.

## Mettre à jour le contenu
Projets, dépôts, compétences et étapes du pipeline sont dans les tableaux
`PROJECTS`, `MINI`, `SKILLS` et `PIPE` en haut du script.
