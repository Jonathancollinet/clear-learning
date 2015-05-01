# Les moments/wizz

Voici le listing de toute les fonctions cloud disponible pour les moments.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Utilité|
| ------------------ | ---------------------------- | ------ |
 eventId | String | ID de l'event
 closed | Boolean | True si l'event est clos
 creator | String **{pointeur '_User'}** | ID du user qui à créer le moment, pointeur vers User
 description | String | Description du moment
 start | String | Date de début ("MM/DD/YYYY HH:MM")
 end | String | Date de fin ("MM/DD/YYYY HH:MM")
 nbParticipant | Number | Nombre de participant actuel.
 nbMaxParticipant | Number | Nombre maximum de participants.
 public | Boolean | True si le moment est public
 title | String | Titre du moment
 picture | String **{pointeur 'Media'}** | ID du Média, photo de couverture, pointeur vers un média voir fiche média et voir doc [parse save file](https://www.parse.com/docs/ios_guide#files/iOS).

##EventAll

/* Liste tous les events */

Pas de paramètres.

Renvoi les paramètres avec un tri du plus récent au plus vieux selon la date de début du wizz.

##EventGetByTitle

/* Get un event par son titre */

Paramètre:

* title

##EventGetById

/* Get un event par son ID */

Paramètres:

* eventId

##EventCreate

/* Créer un event */

Envoyer l'objet complet.

##EventEdit

/* Edite l'event */

Envoyer l'objet complet.

##EventClose

/* Cloture l'event */

Paramètre:

* eventId

##EventRemove

/* Supprime l'event */

Paramètre:

* eventId
