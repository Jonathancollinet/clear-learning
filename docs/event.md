# OK POUR UTILISATION
# Les moments

Voici le listing de toute les fonctions cloud disponible pour les moments.

Le schéma complet:

* objectId | String | ID de l'event
* closed | Boolean | True si l'event est clos
* creator | Objet User | Pointeur vers l'objet user concernant le moment
* description | String | Description du moment
* start | Date | Date de début
* end | Date | Date de fin
* public | Boolean | True si le moment est public
* title | String | Titre du moment
* picture | File | Photo de couverture

##EventAll

/* Liste tous les events */

##EventGetByTitle

/* Get un event par son titre */

##EventGetById

/* Get un event par son ID */

##EventCreate

/* Créer un event */

##EventEdit

/* Edite l'event */

##EventClose

/* Cloture l'event */

##EventRemove

/* Supprime l'event */
