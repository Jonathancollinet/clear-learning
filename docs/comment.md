
# PAS FINI NE PAS ENCORE UTILISER
# Les commentaires

Voici le listing de toute les fonctions cloud disponible pour les commentaires.

Le schéma complet:

* objectId | String | ID du commentaire
* comment | String | Le commentaire
* mediaId | Objet Media | Pointeur vers l'objet média concernant le commentaire
* eventId | Objet Event | Pointeur vers l'objet Event concernant le moment dans lequel se trouve le commentaire
* userId | Objet User | Pointeur vers l'objet User qui à posté le commentaire

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
