# Les likes

Voici le listing de toute les fonctions cloud disponible pour les likes.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Description|
| ------------------ | ---------------------------- | ------ |
 likeId | String | ID du like
 mediaId | String **{pointeur 'Media'}** | ID du média concernant le like
 eventId | String **{pointeur 'Event'}** | ID de l'event concernant le moment dans lequel se trouve le like
 userId | String **{pointeur '_User'}** | ID de l'user qui à liké le média

## LikeCurrentUser

/* Check si le user actuel a liké le média */

Paramètres:

* userId
* mediaId

## LikeAdd

/* Ajoute un like d'un user à un média */

Paramètres:

* eventId
* userId
* mediaId

## LikeRemove

/* Supprime un like d'un user à un média */

Paramètres:

* userId
* mediaId

## LikeRemoveById

/* Supprime un like d'un user à un média par son ID */

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