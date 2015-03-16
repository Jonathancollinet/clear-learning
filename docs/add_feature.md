# Hey i'm the add_feature


## Routes

Pour la plupart des modèles, un *CRUD* est disponible.
Le `:id` correspond à un ID.

> `X` est le nom du modèle

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
