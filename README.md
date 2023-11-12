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

