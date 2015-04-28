# Les moments

Voici le listing de toute les fonctions cloud disponible pour les moments.

Le schéma complet du json à envoyer aux fonctions cloud:

* eventId | String | ID de l'event
* closed | Boolean | True si l'event est clos
* creator | String | Pointeur vers l'objet user concernant le moment
* description | String | Description du moment
* start | String | Date de début ("MM/DD/YYYY HH:MM")
* end | String | Date de fin ("MM/DD/YYYY HH:MM")
* public | Boolean | True si le moment est public
* title | String | Titre du moment
* picture | File | Photo de couverture (voir doc [parse save file](https://www.parse.com/docs/ios_guide#files/iOS))

##EventAll

/* Liste tous les events */

Pas de paramètres.

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
