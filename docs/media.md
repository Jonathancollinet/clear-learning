# Les médias

Voici le listing de toute les fonctions cloud disponible pour les médias.

Le schéma complet du json à envoyer aux fonctions cloud:

* mediaId | String | ID du like
* eventId | String | Pointeur vers l'objet Event concernant le moment dans lequel se trouve le média
* userId | String | Pointeur vers l'objet User qui à liké le média
* title | String | Titre du média
* description | String | Description du média
* file | File | Photo de couverture (voir doc [parse save file](https://www.parse.com/docs/ios_guide#files/iOS))

## MediaAll

/* Liste les média d'un event */

Paramètres:

* eventId

## MediaAdd

/* Ajoute un média a un event */

Paramètres:

* eventId
* userId
* title
* description
* file

## MediaEdit

/* Edite le média */

Paramètres:

* eventId
* userId
* title
* description
* file

## MediaRemove

/* Supprime un média a un event */

Paramètres:

* mediaId

## MediaCountForEvent

/* Compte le nombre de média d'un event */

Paramètres:

* mediaId
