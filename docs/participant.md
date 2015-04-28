# Les participants

Voici le listing de toute les fonctions cloud disponible pour les participants.

Le schéma complet du json à envoyer aux fonctions cloud:

* participantId | String | ID du participant
* eventId | String | Pointeur vers l'objet Event concernant le moment dans lequel se trouve le like
* userId | String | Pointeur vers l'objet User qui à liké le média

## ParticipantList

/* Liste tous les participants d'un event */

Paramètres:

* eventId

## ParticipantAdd

/* Ajoute un participant à l'event */

Paramètres:

* eventId
* userId

## ParticipantRemove

/* Supprime un participant à l'event */

Paramètres:

* participantId

## ParticipantCountForEvent

/* Compte le nombre de participants d'un event */

Paramètres:

* participantId
