### V2.000 du 19/12/2023
-   Nouveau plugin avec fusion d'IOBL et Myhome

### V1.314 du 24/06/2021 20:13
-   Correction d'un bug sur le champ la valeur de la commande vaut par défaut la commande dans l'onglet commande merci à alx68
-   Ajout du template 88200. Merci à alx68 et Figjial
-   Modif du template 67253 en supprimant les commandes locales. Merci à kevinchalet

### V1.313 du 22/11/2020 16:55
-   Correction du type par défaut des index du gestionnaire d'énergie 03809. Merci a Kevin Chalet (PR15)
-   Corrige le chemin du logo In One by Legrand utilisé par défaut dans la vue santé. Merci a Kevin Chalet (PR16)
-   Ajoute une courte attente après chaque envoi de message vers la passerelle USB/CPL. Evite l'ajout de commande sleep entre deux commande d'un scénario. Merci a Kevin Chalet (PR17)
-   Fixe la valeure minimal à 60seconde pour $timersec. Corrige les problèmes avec les interrupteur automatique avec un retour à la normal inferieur a 60s (ne passe pas a Off dans Boxio). Merci a Kevin Chalet (PR18)
-   Vérifie que l'info d'un scénario existe avant de créer un événement associé pour les équipements de type Security. Merci a Kevin Chalet (PR19)
-   Corrige les balises malformées de l'ascenseur Media dans la config de l'equipement (CPL/RF/IR).  Merci a Kevin Chalet (PR20)

### V1.312 du 20/01/2020 20:23
-   Mise a jour de la doc au format Markdown

### V1.311 du 18/11/2019 21:07
-   Mise a jour pour compatibilité jeedom V4

### V1.310 du 04/10/2017 10:11
-   Mise a jour pour compatibilité 3.1.3

### V1.309 du 13/05/2017 22:36
-   Correction du retour d'etat du status Confort (67449)

### V1.308 du 11/05/2017 21:54
-   Implémentation des commandes temporisées (For_time et in_time)

### V1.307 du 10/05/2017 00:25
-   Implémentation  d'un timer de retour auto en low_speed après appui sur high_speed
-   Correction du statut du DIM_STEP
-   Ajout de l'update des prereglages variateur

### V1.306 du 31/02/2017 19:30
-   Mise en place de l'autodetection du port USB utilisé pour l'interface 88213
-   Gestion des onglets dans l'équipement Boxio (Equipement/Commandes/Equipement Pilotés)
-   Ajout de la fonction dupliquer un équipement
-   Suppression des bootstrps
-   Ajout d'un menu Health

### V1.305 du 08/12/2016 20:32
-   Correction du bug de mise a jour d'un equipement lorsqu'il est piloté par lui meme (unit different)
-   Correction du bug d'affichage des equipements pilotés si doublon

### V1.304 du 31/10/2016 14:28
-   Modification des retour d'etat pour les trames Arret et fin_arret (heating)
-   Modification du calcul du type pour la fonction dimensionRequestStatus
-   Ajout d'un timer sur la fonction checkMemory

### V1.303 du 26/10/2016 22:08
-   Correction du demarrage du daemon en mode debug
-   Ajout d'un etat numerique pour les differents modules
-   Correction du retour d'etat des trames DIM_STEP
-   Modification des templates pour faire apparaitre le Nbr d'unit par modules
-   Correction du problèmes de detection des équipements pilotés (cas des modules n'utilisant pas l'unit 2 pour la memoire interne)

### V1.302 du 27/08/2016 17:05
-   Correction d'un bug javascript/Ajax

### V1.301 du 25/08/2016 21:40
-   Ajout de la gestion des statuts des inters scenario
-   Ajout des modules 43214, 67220,77023 et 77024
-   Modification des templates pour intégrer les generic_type (necessaire à l'appli mobile)
-   Ajout de la gestion des statuts pour l'alarme multifonction 43214 
-   Ajout d'une fonction pour mettre à jour les templates via github sans pousser une nouvelle release de boxio
-   Modification de l'affichage de l'equipement pour connaitre la version installée/disponible du template, ainsi qu'une courte description des changements de celle-ci
-   Rajout de la possibilité de lier une commande action a une commande info (necessaire a l'appli mobile)
-   Ajout du mode inclusion (detection auto des modules) dans le plugin (vs config)

### V1.300 du 18/05/2016 22:41
-   Modification du deamon suite aux passages de nginx vers apache=> Résolution du problème de démarrage du plugin avec Jeedom 2.X

### V1.211 du 16/03/2016 22:34
-   Prise en charge de l'equipement 03809
-   Amelioration/Ajouts de retours d'états
-   update du template Management
-   update du template 67215
-   Correction d'un bug dans l'ajout d'un equipement si aucun n'existe

### V1.210 du 26/02/2016 10:40
-   Correction d'un problème sur le retour d'etat des Volets Roulant en mode normal (vs inversé)
-   Ajout de la fonctionnalité d'interrogation du status (Version Beta)
-   Prise en charge de l'équipement 67442(1er version)
-   Correction de bug mineur

### V1.201 du 23/02/2016 20:53
-   Correction d'un problème sur la prise en compte du media dans la trame
-   Correction d'un problème sur la gestion des variateurs (slider)
-   Prise en charge des équipements 67232 et 67214

### V1.200 du 21/02/2016 21:19
-   Implementation de la mise a jour du statut shutter
-   Implementation de la mise a jour du statut lighting
-   Implementation de la mise a jour du statut confort
-   Correction d'un bug sur les équipements pilotés
-   Mise à jour des templates existants
-   Ajout de templates

### V1.102 du 29/11/2015 14:07
-   Modification des templates 67255 et 67251
-   Correction d'un bug d'affichage

### V1.101 du 27/11/2015 22:35
-   Modification des templates "Devices"

### V1.100 du 25/11/2015 21:28
-   Passage en version stable

### V1.007 du 19/11/2015 21:17
-   Correction d'un bug sur le mode Unicast

### V1.006 du 24/10/2015 23:04
-   Correction d'un bug qui bloque l'envoi et la reception de trame quand on demarre le daemon en mode normal (vs debug)
-   Correction d'un bug sur l'ouverture du modal message a partir du plugin
-   Correction pour l'affuchage des logs (Deamon, Daemon.message, Deamon.error et plugin)

### V1.005 du 22/09/2015 23:00
-   Mise à jour du design + Affichage des modules maitre/esclave + modification du daemon et des triggers

### V1.004 du 11/03/2015 00:44
-   Modification du code afin de gérer les units dans les commandes (et non dans l'équipement). Nécessite de supprimer tous les équipements et de les recréer

### V1.003 du 08/03/2015 20:24
-   Ajout des modules 67201 et 67202 (Inter simple et inter double)

### V1.002 du 08/03/2015 09:58
-   Correction d'un bug sur le daemon python
-   Création d'un sous-type inversé pour les modules 67255 et 67251 (en cas d'inversion de l'interrupteur)

### V1.001 du 06/03/2015 19:43
-   Correction du bug d'affichage dans les commandes (mode expert)
-   Correction de l'encodage des fichiers asciidoc
-   Suppression des scripts python superflus

### V1.000 du 05/03/2015 18:15
-   Version initiale

### ToDo
-   Remise a 0 du status au bout d'1 minutes quand Command=ACTION
-   log/debug
-   jeelink
-   Mise a jour doc
-   interpretation des trames d'ack
