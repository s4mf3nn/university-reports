# University Reports

Idée de projet fictif permettant aux élèves et enseignants d'établissements scolaires de remonter des problèmatiques techniques dans les locaux.

## Architecture projet

![Project Architecture](https://user-images.githubusercontent.com/46068217/282327343-f43f4795-3746-4f31-9ba9-80289191f42b.png)

## Réflexion UI/UX
Je partage ici quelque maquettes de l’application. Les maquettes ne sont pas exhaustives, il manque de nombreuses vues, elles servent surtout à présenter une piste de réflexion UI/UX.

## Navigation
Dans la tab bar nous pouvons retrouver 3 items de navigation. Une vue affichant une liste des signalements remontés depuis l’application et qui fera office de page d’accueil. Une vue permettant de créer un nouveau signalement et une vue permettant à l’utilisateur de gérer son compte (paramétrage des notifications push et changement des informations personnelles).

## Vue “Liste des signalements”
On affiche la liste de toutes les demandes d’interventions effectuées depuis l’app. Triées par date, du signalement le plus récent au plus ancien. Pour chaque signalement, on retrouve un lieu, un titre, une catégorie, une date ainsi qu’un état d’avancement (Signalé, En cours de résolution, Résolu). A déterminer si il est utile d’ajouter des options de filtrages (Afficher uniquement les signalements remontés par l’utilisateur connecté, filtrer par état d’avancement).

![reports](https://user-images.githubusercontent.com/46068217/282327514-61802438-c7f2-4cd2-b89b-72617111edb3.png)

## Vue “Signalement”
On affiche dans cette vue le détail d’un signalement crée par un étudiant. Je n’ai pas encore réfléchi à l’intégration de la photo ajouté au signalement mais on retrouve tous les autres éléments essentiels : statut, date et heure, titre, catégorie, lieu, description et activité. L’activité reprend les différentes étapes du traitement de la demande, de la prise en compte, jusqu'à sa résolution. L’activité est matérialisé sous forme de timeline. De l'état le plus récent au plus ancien.

![report](https://user-images.githubusercontent.com/46068217/282327513-f750ac9d-541e-4cec-bf89-4cdbc80dd099.png)

## Vue “Créer un nouveau signalement”
On affiche dans cette vue un formulaire multi-étapes où chaque étape correspond à une seule action afin d’alléger et de simplifier le processus de signalement. On va retrouver 5 étapes : 

Scanner le QRCode du lieu pour démarrer le processus ou renseigner un identifiant unique si le QRCode n’est pas reconnu par le lecteur dans le cas où il serait devenu illisible.

Ajouter un titre au signalement.

Ajouter une description (étape facultative). Champ vide : bouton secondaire “Passer”. Champ renseigné : bouton primaire “Continuer”.

Ajouter une photo (étape facultative). Pas de photo : bouton secondaire “Passer”. Photo uploadé : bouton primaire “Continuer”.

Sélectionner une catégorie parmi :  Panne, Casse, Entretien, Plomberie, Electricité, Thermique (ie. chauffage/clim), Sécurité, Mobilier et Autre.

Une fois le formulaire validé, l’utilisateur est redirigé vers une page confirmant la prise en compte du signalement.

![create-report-step-1](https://user-images.githubusercontent.com/46068217/282327522-8dbd038b-7fca-4532-b1a4-7633b1527493.png)
![create-report-step-2](https://user-images.githubusercontent.com/46068217/282327524-e6678651-5f47-4b5d-bfd7-8dfad299c2d5.png)
![create-report-step-3](https://user-images.githubusercontent.com/46068217/282327525-2c44fc7d-f7ae-4cdc-acdc-1905c3e890a2.png)
![create-report-step-4](https://user-images.githubusercontent.com/46068217/282327526-f75826ac-548b-4880-954d-fbba05eba69b.png)
![create-report-step-5](https://user-images.githubusercontent.com/46068217/282327527-a6541a28-23ee-4048-8dfc-6d9ccafa2ace.png)
![create-report-step-6](https://user-images.githubusercontent.com/46068217/282327509-717ea073-a9e7-42cd-bef8-7e8dbb87b934.png)

## Vue profil (paramètres du compte)
![profile](https://user-images.githubusercontent.com/46068217/282327510-b7051ec8-a75b-4da0-a1e4-4d3564990a3a.png)

## Vue inscription (par numéro de téléphone)
![signup-step-1](https://user-images.githubusercontent.com/46068217/282327516-bd94f67d-e53a-4836-9aab-9f1567edeb63.png)
![signup-step-2](https://user-images.githubusercontent.com/46068217/282327517-14e0b633-2831-4c86-b503-135dc8653394.png)
![signup-step-3](https://user-images.githubusercontent.com/46068217/282327519-759e58ec-7176-45f2-a35b-b419489bd6cd.png)
![signup-step-4](https://user-images.githubusercontent.com/46068217/282327520-d029f2ba-aa1b-4b5a-9bf6-042d47c53f18.png)

## Vue onboarding
TODO

## Avantages de React Native / Expo
Développement multiplateforme simplifié : Expo et React Native permettent de développer une seule base de code pour les applications iOS et Android, ce qui peut réduire les délais ainsi que les coûts de développement.

Accès aux bibliothèques natives : Ces solutions permettent d’accéder aux fonctionnalités natives des appareils (comme l'appareil photo, le GPS, etc.) en utilisant des modules natifs ou des bibliothèques tierces.

Grande communauté et écosystème : React Native a une grande communauté de développeurs (113k étoiles sur Github), de nombreuses bibliothèques tierces et un grand nombre de ressources en ligne.

## ReactJS / PWA
Une Progressive Web App (PWA) est une application web qui combine les fonctionnalités des sites web et des applications mobiles natives. Les PWA sont conçues pour offrir une expérience utilisateur optimale sur les navigateurs web des ordinateurs de bureau et des appareils mobiles, tout en permettant une utilisation hors ligne, une installation sur l'écran d'accueil de l'appareil et un accès aux fonctionnalités matérielles, le tout sans nécessiter de téléchargement depuis un app store.

Accessibilité multi-plateforme : Les PWA sont accessibles via un navigateur web sur différentes plateformes (ordinateurs de bureau, smartphones, tablettes). Il n'est pas nécessaire de développer des applications spécifiques pour chaque plateforme.

Installation simplifiée : Les PWA peuvent être installées sur l'écran d'accueil d'un appareil, offrant une expérience proche de celle d'une application native. Cela se fait en un seul clic, sans avoir à passer par un app store.

Réduction des coûts de développement : Le développement d'une PWA unique pour plusieurs plateformes peut réduire les coûts par rapport au développement et au maintient d’une application mobiles et d’un site web en parallèle.

Flexibilité : ReactJS, est une bibliothèque JavaScript populaire (215k étoiles sur Github) qui offre une grande flexibilité en termes de développement d'interfaces utilisateur et de fonctionnalités.

Communauté active : ReactJS a une communauté de développeurs active et de nombreuses bibliothèques tierces qui facilitent le développement et l'ajout de fonctionnalités à un projet React.

## Notification : Firebase Cloud Messaging
Firebase Cloud Messaging est une solution permettant l’envoi de notifications push sur appareil mobile et web.

Gratuit : FCM est une solution totalement gratuite.

Multiplateforme : FCM prend en charge une variété de plateformes, notamment Android, iOS et le web.

Suivi et analyse des performances : FCM offre des outils de suivi et d'analyse des performances pour vous permettre de mesurer l'efficacité de vos campagnes de notifications push, telles que les taux d'ouverture et de clic.

Sécurité et confidentialité : FCM utilise des connexions sécurisées via HTTPS pour garantir la sécurité des données échangées entre le serveur et les appareils.

Support multi-langues : Vous pouvez envoyer des notifications à la langue de l’utilisateur.

## Authentification par numéro de téléphone mobile : Firebase Auth
Firebase Authentication fournit des SDK et des bibliothèques d'interface utilisateur prêtes à l'emploi pour authentifier les utilisateurs auprès d’une application.

Intégration simplifié : Firebase Auth peut être intégrée dans des applications mobiles et web grâce à des SDK faciles à utiliser.

Vérification des numéros de téléphone : Firebase Authentication propose l’authentification des utilisateurs par l’envoi de SMS et gère la vérification des numéros de téléphone pour s'assurer qu'ils sont valides.

Suivi des performances et des statistiques : Firebase propose des outils de suivi et d'analyse des performances de l'authentification par SMS, y compris des statistiques sur les taux de réussite et les erreurs d'authentification.

Multiplateforme : Le service est utilisable sur Android, iOS et Web, ce qui permet de proposer une expérience d'authentification cohérente à travers ces différentes plateformes.
