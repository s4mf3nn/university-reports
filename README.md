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
