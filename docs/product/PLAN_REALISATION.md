# Délice Diet — Plan de réalisation

Date : 16 novembre 2026

## Objectif

Créer la vitrine publique du cabinet de nutrition et de diététique Délice Diet, adaptée en priorité aux téléphones. Le visiteur doit comprendre les prestations, découvrir le cabinet et demander un rendez-vous auprès de celui-ci.

Le brief et le prototype `index.html` constituent les références fonctionnelle et visuelle. Les images de consultation et de repas sont des illustrations générées. Les prestations, coordonnées et informations du praticien doivent être confirmées avant leur publication.

## État actuel

- Dépôt Git initialisé, sans commit au moment de la rédaction.
- Brief, logo, images et prototype HTML autonome disponibles.
- Le prototype comprend les sections principales, un menu mobile et un parcours de contact provisoire.
- Le rendu du prototype reste à vérifier dans un navigateur. Aucune application SvelteKit ni dépendance du projet n'est encore initialisée.

## Choix techniques

| Technologie | Rôle |
| --- | --- |
| SvelteKit et Svelte | Structure de l'application, routes et composants. |
| TypeScript | Typage des données de contenu et des interactions. |
| Tailwind CSS | Styles, palette, mise en page et adaptation aux écrans. |
| shadcn-svelte | Composants d'interface adaptés à Svelte, personnalisés selon la charte. Ajouter uniquement ceux nécessaires. |
| Lucide pour Svelte | Icônes cohérentes, importées selon les besoins. |

Le cabinet a besoin d'une page vitrine. La génération statique avec `@sveltejs/adapter-static` est proposée pour la première version, sous réserve de vérifier les exigences de l'hébergeur retenu. Le site reste indépendant du logiciel de gestion.

Utiliser npm et son fichier de verrouillage comme choix de travail provisoire. Déterminer les versions compatibles lors de l'initialisation et documenter la version de Node nécessaire. Les composants shadcn-svelte sont intégrés au code du projet et adaptés à la charte.

## Architecture proposée

L'arborescence suivante guide l'implémentation. Les fichiers seront créés au fur et à mesure de leur utilité.

```text
delice-diet-site/
├── src/
│   ├── app.html
│   ├── app.css
│   ├── lib/
│   │   ├── components/
│   │   │   ├── ui/                # Composants shadcn-svelte utilisés
│   │   │   └── sections/          # En-tête, accueil, prestations, cabinet, contact, pied de page
│   │   ├── content/               # Textes et coordonnées validés
│   │   └── assets/                # Images importées et traitées par Vite si pertinent
│   └── routes/
│       ├── +layout.svelte
│       ├── +layout.ts             # Prérendu si génération statique retenue
│       └── +page.svelte
├── static/                        # Ressources publiques nécessitant une URL stable
├── docs/product/PLAN_REALISATION.md
├── BRIEF_LANDING_PAGE_DELICE_DIET.md
├── index.html                     # Prototype autonome de référence
├── package.json
├── svelte.config.js
├── tsconfig.json
└── vite.config.ts
```

Les données publiques du cabinet et la construction du lien de rendez-vous seront regroupées dans un emplacement lisible. Les numéros et coordonnées restent vides tant qu'ils ne sont pas confirmés. La navigation doit conserver une solution utilisable sur mobile et au clavier.

## Étapes de réalisation

### 1. Initialisation et base technique

- Initialiser SvelteKit avec TypeScript dans le dépôt existant, sans écraser le prototype ni les ressources.
- Configurer Tailwind, shadcn-svelte et Lucide, puis ajouter les scripts de développement, vérification et build.
- Configurer le prérendu et l'adaptateur statique si les conditions de déploiement le permettent.
- Documenter l'installation et le lancement local.

**Acceptation** : installation reproductible, serveur de développement opérationnel, vérification TypeScript et build réussis. Le prototype existant reste accessible.

### 2. Charte et structure de page

- Définir les couleurs du prototype sous forme de variables de thème : vert `#095501`, orange `#F56202`, ivoire `#FAF8F1`, sauge `#EAF2E6`, encre `#172317`, blanc et vert profond.
- Intégrer le logo, les photographies d'illustration et les styles de verre dépoli.
- Reproduire l'en-tête, l'accueil, les prestations, le cabinet, le contact et le pied de page avec des composants adaptés au contenu.
- Optimiser les images et prévoir leurs alternatives textuelles.

**Acceptation** : page cohérente avec le prototype et les références sur mobile, tablette et ordinateur, sans débordement horizontal, avec une hiérarchie de contenu lisible.

### 3. Navigation et rendez-vous

- Relier la navigation aux sections et rendre le menu mobile accessible au clavier.
- Centraliser le canal et les coordonnées confirmés. Si WhatsApp est choisi, ouvrir une demande préremplie. Si l'appel est choisi, utiliser un lien téléphonique.
- Tant que le canal n'est pas confirmé, conserver une indication claire et le message à copier, sans annoncer une réservation.

**Acceptation** : liens et menu utilisables au clavier et au toucher. Après configuration, le bouton ouvre le bon canal et la bonne destination sur un téléphone. Tester séparément l'état sans coordonnées.

### 4. Contenus, référencement et vérifications

- Faire confirmer les prestations, la présentation du praticien, la ville, l'adresse, les horaires et les coordonnées.
- Renseigner le titre, la description, la langue et les métadonnées de partage. Ajouter l'image de partage et l'URL publique après choix du domaine.
- Vérifier le contraste, le focus visible, les images, les ancres, les interactions et la préférence de réduction des animations.
- Vérifier le rendu et le parcours réel dans un navigateur sur les formats pertinents, puis relancer les vérifications et le build.

**Acceptation** : informations relues par le cabinet, aucun lien fictif dans la version publique et parcours de contact vérifié avec les coordonnées réelles.

### 5. Préparation de la mise en ligne

- Choisir le domaine et l'hébergement avec le cabinet.
- Adapter la sortie de build à l'hébergement choisi, tester la version générée et vérifier le domaine, les liens et l'aperçu de partage.
- Déployer lorsque la mise en ligne sera demandée et les informations confirmées.

## Informations à confirmer

1. Prestations exactes et présentation du praticien.
2. Ville, adresse, horaires et coordonnées publiques.
3. Canal de rendez-vous et numéro international associé.
4. Photographie autorisée du cabinet ou du praticien, si elle doit remplacer l'illustration.
5. Domaine et hébergement.

## Références techniques

Documentation consultée le 16 novembre 2026.

- [Installation de Tailwind CSS avec SvelteKit](https://tailwindcss.com/docs/installation/framework-guides/sveltekit)
- [Installation de shadcn-svelte avec SvelteKit](https://www.shadcn-svelte.com/docs/installation/sveltekit)
- [Adaptateurs SvelteKit](https://svelte.dev/docs/kit/adapters)
- [Paquets Lucide](https://lucide.dev/packages)
