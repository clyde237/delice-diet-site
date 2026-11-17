# Délice Diet

Site vitrine du cabinet de nutrition et de diététique Délice Diet.

## Développement local

Node.js 20.19+ ou 22.12+ est requis par Vite 7. Installer les dépendances puis lancer le serveur :

```bash
npm install
npm run dev
```

Pour vérifier les types et générer le site statique :

```bash
npm run check
npm run build
npm run preview
```

La sortie statique se trouve dans `build/`. Le prototype autonome existant reste dans `index.html`. Le plan de réalisation se trouve dans `docs/product/PLAN_REALISATION.md`.

## Déploiement sur Vercel

Importer le dépôt GitHub dans Vercel et sélectionner sa racine comme répertoire du projet. Le fichier `vercel.json` configure l'installation avec `npm ci`, la compilation avec `npm run build` et la publication du dossier statique `build/`. Il choisit le préréglage « Other », car la sortie est produite par `adapter-static`.

Dans les paramètres du projet Vercel, choisir une version de Node.js compatible avec Vite 7, par exemple Node.js 22. Les prochains commits poussés sur la branche de production déclenchent un nouveau déploiement lorsque l'intégration Git est active.
