# Les utilisateurs

Voir la documentation de [Parse](http://www.parse.com) selon le SDK sur lequel vous travaillez.

Si vous faites de l'IOS, voir la documentation de parse IOS.

Voir ensuite la documentation lié aux USERS.

Toutes les informations relatives au login/signup reset password etc etc etc, l'envoi de mail est déjà géré par Parse, elle est désactivé par défault et nous pouvons l'activer sur demande.

<img src="../images/doc_ios.jpeg" alt="Doc" style="width: 400px;"/>

# Fonction custom

----------------------
## User.beforeSave
----------------------

* check si le true_username est bien formaté et si il n'est pas déjà existant

----------------------
## UserGetById
----------------------

**Pagination disponible**

*Get infos d'un user par son id*

Paramètres:

* userId

----------------------
## UserGetFollowing
----------------------

**Pagination disponible**

*Get les following d'un user, renvoi les donnée sous la forme d'un array d'User*

Renvoi les resultats trié par createdAt descendant.

Paramètres:

* userHim

----------------------
## UserGetFollowed
----------------------

**Pagination disponible**

*Get les followed d'un user, renvoi les donnée sous la forme d'un array d'User*

Renvoi les resultats trié par createdAt descendant.

Paramètres:

* userHim

----------------------
## UserGetByTrueUsername
----------------------

*Get infos d'un user par son true_username*

Paramètres:

* true_username
