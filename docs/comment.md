# Les commentaires

Voici le listing de toute les fonctions cloud disponible pour les commentaires.

Le schéma:

* objectId | String | ID du commentaire
* comment | String | Le commentaire
* mediaId | Objet Media | 
* eventId | Objet Event |
* userId | Objet User
* createdAt | String
* updatedAt | String

##CommentAll

/* Liste tous les commentaires d'un event */

##CommentAllForUser

/* Liste tous les commentaires d'un user d'un event */

##CommentAdd

/* Ajoute un commentaires d'un user */

##CommentRemove

/* Supprime un commentaires d'un user */

##CommentCountForMedia

/* Compte le nombre de commentaires d'un média */

##CommentCountForEvent

/* Compte le nombre de commentaires d'un event */
