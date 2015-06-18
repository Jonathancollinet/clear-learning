# Les notifications

Voici le listing de toute les fonctions cloud disponible pour les notif friend.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Description|
| ------------------ | ---------------------------- | ------ |
 from | String | ID du User qui fait la demande
 to | String | ID du User qui reçoit la demande
 eventId | String **{pointeur 'Event'}** | id vers l'event concerné si c'est le cas
 participantId | String **{pointeur 'Participant'}** | id vers la participation concerné si c'est le cas
 viewed | Boolean | Savoir si le user a vu la notif.
 type | String | Type de la notification ('alert' pour les alertes*, 'invite' pour les invitation**, 'response' pour les réponses***)
 content | String | Contenu de la notification
 link | String | Lien vers lequel l'utilisateur sera redirigé lorsqu'il cliquera sur la notif

----------------------
##N_Add
----------------------

/*Créer une notification*

Paramètres:

Renseigner les champs ci-dessus;

Les variables 'link', 'friendId', 'participantId' sont optionnelles.

----------------------
##N_GetAlert
----------------------

**Pagination disponible**

*Récupère les alertes du current*

Pas de paramètres.

----------------------
##N_GetInvite
----------------------

**Pagination disponible**

*Récupère les invitations du current*

Pas de paramètres.

----------------------
##N_Viewed
----------------------

*Set viewed à true*

Paramètres:

* nId (id de la notif)

----------------------
##N_Remove
----------------------

*remove une notif*

Paramètres:

* nId (id de la notif)
