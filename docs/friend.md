# Les Amis

Voici le listing de toute les fonctions cloud disponible pour les friend.

----------------------

**following**: **X si X suit Y**

**followed**: **X si X est suivi par Y**

----------------------

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Description|
| ------------------ | ---------------------------- | ------ |
 userHim | String | ID du User qui suit
 userHas | String | ID du User qui est suivi

----------------------
##FriendCountFollowing
----------------------

/* Compte les following d'un user */

Paramètres:

* userHim

----------------------
##FriendCountFollowed
----------------------

/* Compte les followed d'un user */

Paramètres:

* userHim

----------------------
##FriendGetFollowingByUser
----------------------

/* Liste les following d'un user */

Paramètres:

* userHim

Renvoi les données avec un tri du plus récent au plus vieux selon la date de création.

----------------------
##FriendGetFollowedByUser
----------------------

/* Liste les followed d'un user */

Paramètres:

* userHim

Renvoi les données avec un tri du plus récent au plus vieux selon la date de création.

----------------------
##FriendAdd
----------------------

/* Ajoute un following a un user */

Créer une liaison entre userHim et userHas.

**Vous devez effectuer une deuxième requete pour ajouter la liaison avec l'autre ami**

Paramètres:

* userHim
* userHas

----------------------
##FriendRemoveByUser
----------------------

/* Supprime un following d'un user avec les deux ID */

**Supprime la liaison dans les deux sens donc pas besoin de l'appeler deux fois.**

Paramètres:

* userHim
* userHas

----------------------
##FriendRemoveById
----------------------

/* Supprime un following d'un user par l'id de l'objet friend */

Paramètres:

* friendId

