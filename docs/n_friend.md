# Les Notifications d'amis

Voici le listing de toute les fonctions cloud disponible pour les notif friend.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Description|
| ------------------ | ---------------------------- | ------ |
 userHim | String | ID du User qui fait la demande
 userFor | String | ID du User qui reçoit la demande
 status | String | Status de la notification ('accepted', 'pending', 'refused')

----------------------
##N_FriendGetForUser
----------------------

/* Liste les demande d'ajout d'ami d'un user */

Paramètres:

* userHim

Renvoi les données avec un tri du plus récent au plus vieux selon la date de création.

----------------------
##N_FriendAdd
----------------------

/* Créer une demande d'ajout d'ami */

Paramètres:

* userHim
* userFor

----------------------
##N_FriendSetStatus
----------------------

/* Change le status d'une demande d'ajout d'ami */

Paramètres:

* userHim
* userFor

----------------------
##N_FriendRemoveByUser
----------------------

/* Supprime une demande d'ajout d'ami par les user */

Paramètres:

* userHim
* userHas

----------------------
##N_FriendRemoveById
----------------------

/* Supprime une demande d'ajout d'ami par l'id de la notif */

Paramètres:

* n_friendId

