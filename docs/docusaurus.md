---
sidebar_position: 1
sidebar_label: 'Docusaurus démo'
---

1. Lancer le starter + lancer l'app de démo
```
npx create-docusaurus@latest docusaurus-demo classic --typescript

cd docusaurus-demo
npm start
```

2. Initialiser Git puis pousser
```
git init -b main

git add .
git commit -m 'feat: initial commit'

git remote add origin git@github.com:josephpage/docusaurus-demo.git
git branch -M main
git push -u origin main
```

3. Ouvrir dans VSCode
```
code .
```

- Changer un bon de la configuration dans `docusaurus.config.js` :
```
// Set the production url of your site here
url: 'https://josephpage.github.io/',
// Set the /<baseUrl>/ pathname under which your site is served
// For GitHub pages deployment, it is often '/<projectName>/'
baseUrl: '/docusaurus-demo/',

// GitHub pages deployment config.
// If you aren't using GitHub pages, you don't need these.
organizationName: 'josephpage', // Usually your GitHub org/user name.
projectName: 'docusaurus-demo', // Usually your repo name.
```
- Remplacer toutes les occurences de `facebook/docusaurus` dans le projet.
- `git add . && git commit -m "feat: publish with Github Pages" && git push`

4. Activer Github Pages dans les Settings du repo sur Github.com (branche "gh-pages" avec "/")

4. Déployer sur Github Pages
```
npm run deploy
# => va déployer instantanément sur Github Pages à travers gh-pages
```

