# Délice Diet — Brief de la landing page

## Contexte et objectif

Délice Diet est un cabinet de nutrition et de diététique au Cameroun. Son logiciel de gestion interne, `Delice-App-main`, est en cours de développement. La priorité est de créer la vitrine publique du cabinet dans le projet indépendant `delice-diet-site`, avec son propre dépôt et son propre déploiement.

La première version doit permettre à un futur patient de comprendre les prestations du cabinet, de trouver ses coordonnées et de demander un rendez-vous facilement depuis son téléphone.

## Périmètre de la page

| Section | Contenu attendu |
| --- | --- |
| En-tête | Logo et liens vers les prestations, le cabinet et le contact. |
| Accueil | Nom Délice Diet, présentation en une phrase et bouton « Prendre rendez-vous ». |
| Prestations | Présentation des services confirmés. La consultation initiale et le suivi diététique sont des pistes à valider. |
| Le cabinet | Approche du cabinet, présentation du praticien et photo si elle est fournie et autorisée. |
| Informations pratiques | Adresse, horaires, coordonnées et lien d’itinéraire si l’adresse est confirmée. |
| Pied de page | Identité du cabinet et liens utiles. |

## Parcours de rendez-vous

Le bouton « Prendre rendez-vous » ouvre le canal retenu par le cabinet, par exemple un appel ou WhatsApp. Si WhatsApp est choisi, prévoir un message simple comme « Bonjour, je souhaite prendre rendez-vous pour une consultation. » Le créneau est convenu directement avec le cabinet.

Cette version couvre la vitrine et le contact. L’agenda en ligne, les comptes patients, les paiements et l’intégration au logiciel de gestion pourront être cadrés plus tard. La page ne collecte aucune donnée médicale.

## Direction et réalisation

- Rédiger en français. Reprendre le logo officiel et ses couleurs dès que les fichiers sont fournis. Privilégier une mise en page claire, aérée et adaptée au mobile.
- Partir sur une page statique et légère. Le choix de la technologie reste ouvert. Documenter le lancement local dans le dépôt.
- Optimiser les images et prévoir un titre de page, une méta-description et un aperçu de partage.
- Tester la lisibilité sur mobile et ordinateur, les contrastes, la navigation clavier et le lien de prise de rendez-vous.

## Informations à confirmer avant publication

- Logo, couleurs officielles et visuels disponibles.
- Prestations et présentation du praticien à publier.
- Ville, adresse, horaires et coordonnées publiques.
- Canal principal de prise de rendez-vous et numéro ou lien correspondant.
- Nom de domaine et hébergement, si déjà choisis.

Pendant le prototypage, signaler les contenus à confirmer. Utiliser uniquement les informations validées dans la version publiée.

## Ordre de travail et critères de livraison

1. Vérifier le dépôt `delice-diet-site` et initialiser Git si nécessaire.
2. Rassembler les contenus et confirmer le canal de prise de rendez-vous.
3. Concevoir puis réaliser la page responsive.
4. Tester le parcours depuis le bouton de rendez-vous jusqu’au bon contact et faire relire les informations publiques avant publication.

La page est livrable quand un visiteur peut identifier le cabinet, comprendre ses services et le joindre depuis son téléphone. Le dépôt contient la page et les instructions de lancement local.
