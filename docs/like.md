# Les likes

Voici le listing de toute les fonctions cloud disponible pour les likes.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Description|
| ------------------ | ---------------------------- | ------ |
 likeId | String | ID du like
 mediaId | String **{pointeur 'Media'}** | ID du média concernant le like
 eventId | String **{pointeur 'Event'}** | ID de l'event concernant le moment dans lequel se trouve le like
 userId | String **{pointeur '_User'}** | ID de l'user qui à liké le média

----------------------
## Like.afterSave
----------------------

* Incrément le nombre de likes lié au média

----------------------
## LikeCurrentUser
----------------------

/* Check si le user actuel a liké le média */

Paramètres:

* userId
* mediaId

Renvoi:

	{liked: true, mediaId: "IOi7mMdz"}

----------------------
## LikeAdd
----------------------

/* Ajoute un like d'un user à un média */

Paramètres:

* eventId
* userId
* mediaId

----------------------
## LikeGetByArrayMedia
----------------------

/* Renvoi les média que le current user à liké dans un set de média donné */

Paramètres:

* mediaIds -> correspond à un array contenant des objets Media

----------------------
## LikeRemove
----------------------

/* Supprime un like d'un user à un média */

Décrémente le nbLike de l'objet Media dans lequel se trouve le like

Paramètres:

* userId
* mediaId

----------------------
## LikeRemoveById
----------------------

/* Supprime un like d'un user à un média par son ID */

Décrémente le nbLike de l'objet Media dans lequel se trouve le like

Paramètres:

* likeId

----------------------
## LikeCountForMedia
----------------------

**(ATTENTION, FONCTION LENTE ET LIMITEE, VEUILLEZ UTILISER LE CHAMPS nbLike DANS L'OBJET MEDIA)**

/* Compte le nombre de likes d'un média */

Paramètres:

* eventId
* mediaId

----------------------
## LikeCountForEvent
----------------------

**(ATTENTION, FONCTION LENTE ET LIMITEE, VEUILLEZ LIMITER LUTILISATION DE CETTE FONCTION)**

/* Compte le nombre de likes d'un event */

Paramètres:

* eventId