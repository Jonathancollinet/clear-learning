
# Les commentaires

Voici le listing de toute les fonctions cloud disponible pour les commentaires.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Utilité|
| ------------------ | ---------------------------- | ------ |
 commentId | String | ID du commentaire
 comment | String | Le commentaire
 mediaId | String **{pointeur 'Media'}** | ID du média concernant le commentaire
 eventId | String **{pointeur 'Event'}** | ID de l'event concernant le moment dans lequel se trouve le commentaire
 userId | String **{pointeur '_User'}** | ID de l'user qui à posté le commentaire

##CommentAll

/* Liste tous les commentaires d'un event */

Paramètres:

* eventId
* mediaId

##CommentAllForUser

/* Liste tous les commentaires d'un user d'un event */

Paramètres:

* eventId
* userId
* mediaId

##CommentAdd

/* Ajoute un commentaires d'un user */

Paramètres:

* eventId
* userId
* mediaId
* comment

##CommentRemove

/* Supprime un commentaires d'un user */

Paramètres:

* commentId

##CommentCountForMedia

/* Compte le nombre de commentaires d'un média */

Paramètres:

* eventId
* mediaId

##CommentCountForEvent

/* Compte le nombre de commentaires d'un event */

Paramètres:

* eventId
