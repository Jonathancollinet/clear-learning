# Les médias

Voici le listing de toute les fonctions cloud disponible pour les médias.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Description|
| ------------------ | ---------------------------- | ------ |
 mediaId | String | ID du like
 eventId | String **{pointeur 'Event'}** | ID du moment concernant le moment dans lequel se trouve le média
 userId | String **{pointeur '_User'}** | ID de qui à liké le média
 title | String | Titre du média
 nbLike | Number | Nombre de like actuel.
 nbComment | Number | Nombre de comment actuel.
 description | String | Description du média
 type | String | Type du média ('photo', 'video', 'texte', 'gif', 'audio')
 file | File | Photo de couverture (voir doc [parse save file](https://www.parse.com/docs/ios_guide#files/iOS))


----------------------
## Media.afterSave
----------------------

* Incrément le nombre de médias lié à l'évènement

----------------------
## Media.afterDelete
----------------------

* Décrémente le nombre de médias lié à l'évènement
* Supprime les commentaires liés au média
* Supprime les likes liés au média
* Supprime le média et la miniature (si existant) des fichiers

----------------------
## MediaAll
----------------------

**Pagination disponible**

*Liste les média d'un event*

Paramètres:

* eventId

----------------------
## MediaAdd
----------------------

*Ajoute un média a un event*

Paramètres:

* eventId
* userId
* title
* description
* file

----------------------
## MediaEdit
----------------------

*Edite le média*

Paramètres:

* eventId
* userId
* title
* description
* file

----------------------
## MediaRemove
----------------------

*Supprime un média a un event*

Paramètres:

* mediaId

----------------------
## MediaCountForEvent
----------------------

*Compte le nombre de média d'un event*

Paramètres:

* mediaId
