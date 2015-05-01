# Les participants

Voici le listing de toute les fonctions cloud disponible pour les participants.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Utilité|
| ------------------ | ---------------------------- | ------ |
 participantId | String | ID de la participation
 eventId | String **{pointeur 'Event'}** | ID de l'event auquel le participant participe
 userId | String **{pointeur '_User'}** | ID de l'user qui participe, pointeur ver l'user

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
