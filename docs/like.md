# Les likes

Voici le listing de toute les fonctions cloud disponible pour les likes.

Le schéma complet du json à envoyer aux fonctions cloud:

* likeId | String | ID du like
* mediaId | String | Pointeur vers l'objet média concernant le like
* eventId | String | Pointeur vers l'objet Event concernant le moment dans lequel se trouve le like
* userId | String | Pointeur vers l'objet User qui à liké le média

## LikeAdd

/* Ajoute un like d'un user à un média */

Paramètres:

* eventId
* userId
* mediaId

## LikeRemove

/* Supprime un like d'un user à un média */

Paramètres:

* likeId

## LikeCountForMedia

/* Compte le nombre de likes d'un média */

Paramètres:

* eventId
* mediaId

## LikeCountForEvent

/* Compte le nombre de likes d'un event */

Paramètres:

* eventId