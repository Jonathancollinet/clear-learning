# Les Amis

Voici le listing de toute les fonctions cloud disponible pour les friend.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Utilité|
| ------------------ | ---------------------------- | ------ |
 userHim | String | ID du User qui fait la demande
 userHas | String | ID du User qui reçoit la demande

##FriendGetByUser

/* Liste les amis d'un user */

Paramètres:

* userHim

Renvoi les données avec un tri du plus récent au plus vieux selon la date de création.

##FriendAdd

/* Ajoute un ami a un user */

Créer une liaison entre userHim et userHas.
**Vous devez effectuer une deuxième requete pour ajouter la liaison avec l'autre ami**

Paramètres:

* userHim
* userHas

##FriendRemoveByUser

/* Supprime un ami d'un user avec les deux ID */

Paramètres:

* userHim
* userHas

##FriendRemoveById

/* Supprime un ami d'un user par l'id de la liaison */

Paramètres:

* userHim
* userHas

