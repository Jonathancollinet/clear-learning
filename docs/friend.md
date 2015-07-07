# Les Amis

Voici le listing de toute les fonctions cloud disponible pour les friend.

----------------------

**following**: **X si X suit Y**

**followed**: **X si X est suivi par Y**

Plus simplement: userHim -> from ; userHas -> to

----------------------

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Description|
| ------------------ | ---------------------------- | ------ |
 userHim | String | ID du User qui suit
 userHas | String | ID du User qui est suivi
 status | String | 'pending', 'accepted', ('refused' -> pour le moment on delete le friend si c'est ce cas)

----------------------
##FriendSearchFollowing
----------------------

*Récupère une liste de potentiel following en excluant lui meme et ses amis*

Paramètres:

* search

----------------------
##FriendIsPending
----------------------

*check si le currentUser à une demande en attente sur le user to*

Paramètres:

* userHas
* search

----------------------
##FriendHasPending
----------------------

*check si le currentUser à une demande en attente sur le user to*

Paramètres:

* userHim

----------------------
##FriendSetStatus
----------------------

*Set le status ("accepted", "refused", "pending")*

Paramètres:

* friendId
* status

ou

* userHim
* userHas
* status

----------------------
##FriendIsFollowing
----------------------

*True/False si userHim suit userHas*

Paramètres:

* userHim
* userHas

----------------------
##FriendIsFollowed
----------------------

*True/False si userHim est suivi par userHas*

Paramètres:

* userHim
* userHas

----------------------
##FriendCountFollowing
----------------------

*Compte les following d'un user*

Paramètres:

* userHim

----------------------
##FriendCountFollowed
----------------------

*Compte les followed d'un user*

Paramètres:

* userHim

----------------------
##FriendGetFollowingByUser
----------------------

**Pagination disponible**

*Liste les following d'un user*

Paramètres:

* userHim

Renvoi les données avec un tri du plus récent au plus vieux selon la date de création.

----------------------
##FriendGetFollowedByUser
----------------------

**Pagination disponible**

*Liste les followed d'un user*

Paramètres:

* userHim

Renvoi les données avec un tri du plus récent au plus vieux selon la date de création.

----------------------
##FriendAdd
----------------------

*Ajoute un following a un user*

Créer une liaison entre userHim et userHas.

**Vous devez effectuer une deuxième requete pour ajouter la liaison avec l'autre ami**

Paramètres:

* userHim
* userHas

----------------------
##FriendRemoveByUser
----------------------

*Supprime un following d'un user avec les deux ID*

**Supprime la liaison dans les deux sens donc pas besoin de l'appeler deux fois.**

Paramètres:

* userHim
* userHas

