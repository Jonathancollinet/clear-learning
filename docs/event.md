# Les moments/wizz/event

Voici le listing de toute les fonctions cloud disponible pour les moments.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Description|
| ------------------ | ---------------------------- | ------ |
 eventId | String | ID de l'event
 closed | Boolean | True si l'event est clos
 creator | String **{pointeur '_User'}** | ID du user qui à créer le moment, pointeur vers User
 city | String | Ville du moment
 description | String | Description du moment
 start | String | Date de début ("MM/DD/YYYY HH:MM Z")
 end | String | Date de fin ("MM/DD/YYYY HH:MM Z")
 nbMedia | Number | Nombre de media actuel dans le moment.
 nbParticipant | Number | Nombre de participant actuel.
 nbMaxParticipant | Number | Nombre maximum de participants.
 public | Boolean | True si le moment est public
 title | String | Titre du moment
 picture | String **{pointeur 'Media'}** | ID du Média, photo de couverture, pointeur vers un média voir fiche média et voir doc [parse save file](https://www.parse.com/docs/ios_guide#files/iOS).
 author_approval | Boolean | True/false si l'option 'sur acceptation du créateur' est activée.
 sharing | Boolean | True/false si l'option 'partage autorisé' est activée.


----------------------
##Event.afterDelete
----------------------

* Supprime tous les [médias](media.md#mediaafterdelete) liés à l'évènement

----------------------
##EventAll
----------------------

**Pagination disponible**

/* Liste tous les events */

Pas de paramètres.

Renvoi les paramètres avec un tri du plus récent au plus vieux selon la date de début du wizz.

----------------------
##EventCount
----------------------

/* Compte tous les events */

Pas de paramètres.

----------------------
##EventGetByTitle
----------------------

**Pagination disponible**

/* Get un event par son titre */

Paramètre:

* title

----------------------
##EventGetByCreator
----------------------

**Pagination disponible**

/* Get les event par le creator */

Paramètre:

* creator

----------------------
##EventGetParticipating
----------------------

**Pagination disponible**

/* Get les event auquel l'utilisateur courant participe */

Paramètre: null

----------------------
##EventGetByUser
----------------------

**Pagination disponible**

/* Get les event par l'userId */

Paramètre:

* userId

----------------------
##EventGetByCity
----------------------

**Pagination disponible**

/* Get un event par sa ville */

Paramètre:

* city

----------------------
##EventGetById
----------------------

/* Get un event par son ID */

Paramètres:

* eventId

----------------------
##EventCreate
----------------------

/* Créer un event */

Envoyer le schéma JSON complet.

----------------------
##EventEdit
----------------------

/* Edite l'event */

Envoyer le schéma JSON complet.

----------------------
##EventClose
----------------------

/* Cloture l'event */

Paramètre:

* eventId

----------------------
##EventOpen
----------------------

/* Open l'event */

Paramètre:

* eventId

----------------------
##EventRemove
----------------------

/* Supprime l'event */

Paramètre:

* eventId

---------------------
##EventGetLast
---------------------

/* Get le last event auquel le current participe et qui est encore ouvert/pas terminé */

Pas de paramètres.

