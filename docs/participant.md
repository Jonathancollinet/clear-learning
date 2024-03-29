# Les participants

Voici le listing de toute les fonctions cloud disponible pour les participants.

Le schéma complet du json à envoyer aux fonctions cloud:

Nom de la variable | Type attendu                 | Description
------------------ | ---------------------------- | ------
 participantId | String | ID de la participation
 eventId | String **{pointeur 'Event'}** | ID de l'event auquel le participant participe
 userId | String **{pointeur '_User'}** | ID de l'user qui participe, pointeur ver l'user
 status | String | Status de la participation ('accepted', 'pending', 'refused')
 invited | Boolean | Savoir si ce participant a été invité par le créateur
 approval | Boolean | Savoir si le créateur à accepté la demande d'inscription à un evenement

----------------------
## ParticipantList
----------------------

**Pagination disponible**

*Liste tous les participants d'un event*

Paramètres:

* eventId

----------------------
## ParticipantAdd
----------------------

*Ajoute un participant à l'event*

Paramètres:

* eventId
* userId

----------------------
## ParticipantIsPending
----------------------

*Renvoi l'objet si le current user a une participation en attente sur un event, sinon renvoi false*

Paramètres:

* userId
* eventId

----------------------
## ParticipantSetStatus
----------------------

*Set le status ("accepted", "refused", "pending")*

Si paramètre status == 'accepted' alors le Event.nbParticipant += 1;

Paramètres:

* participantId
* status

ou

* userId
* eventId
* status

----------------------
## ParticipantRemove
----------------------

*Supprime un participant à l'event*

Paramètres:

* participantId

----------------------
## ParticipantCountForEvent
----------------------

**(ATTENTION, FONCTION LENTE ET LIMITEE, VEUILLEZ UTILISER LE CHAMPS nbParticipant DANS L'OBJET EVENT)**

*Compte le nombre de participants d'un event*

Paramètres:

* participantId

