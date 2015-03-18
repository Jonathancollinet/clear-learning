## Architecture et implémentation

	A reflechir sur l'api
	dédié/ & partagé/

	Les fichiers dédié contiendrai des donnée relatives a un model
	Les fichiers partagé contiendrai des données génériques réutilisé dans l'ensemble du back.

Dans le dossier `api/` situé à la racine, créer un dossier `X/` qui va ensuite contenir un fichier `crud.js` ou `index.js` [A CONFIRMER].

Ce fichier contiendra toutes les méthodes concernant le modèle fais de la façon suivante:

	exports.methodName = function(req, res, next) {
			
				----fais du stuff----

	};

Il faut ensuite créer les routes dans le fichier `routes.js`.
Voir ci-dessus les routes.

## Routes

Pour la plupart des modèles, un *CRUD* est disponible.
Bien entendu, chaque modèles peut disposer de *méthodes spécifiques* à eux-même.
Pour ce cas, nous créerons un fichier **nommé contextuellement**.

> `:id` correspond à un ID

*POST* -> CREATE

* `/X` : créer un X

*GET* -> READ

* `/X/findOne` : renvoi un X.
* `/X/count` : renvoi le nombre de X.
* `/X/:id` : renvoi l'id depuis X.
* `/X/:id/exists` : renvoi si l'id depuis X existe.

*PUT* -> UPDATE

* `/X/:id` : met à jour l'id depuis X.

*REMOVE* -> DELETE

* `/X/:id` : supprime l'id depuis X.

