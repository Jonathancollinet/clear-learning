# clear-learning
Documentation WiZZeM

## Install mkdocs
http://www.mkdocs.org/#installation

### 14/05

* ajout de nbFollowing & nbFollower dans l'objet User qui permette d'éviter de faire des counts du côté des Friends

### 13/05

* La date de fin d'un moment n'est plus setable, elle est défini a : DateStart + 1 mois

### 12/05

* ajout des fonctions custom dans la partie User.

### 11/05

* Ajout de colonnes: Event:[nbMedia], Media:[nbLike, nbComment]

Auto incrémente/décrémente lors d'une création ou destruction, directement dans les objets.

Attention, éviter d'utiliser les fonctions count, veuillez utiliser les compteurs directement dans les objets global (get le nombre de like ? Non plus count dans Like, mais get('nbLike') dans l'objet Media).

### 10/05

* ajout des codes d'erreur

### 09/05

(2)

* ajout d'une fonction friend.

(1)

* modification des friends -> follow
* lecture plus fluide

### 08/05

(2)

* Ajout des notifications friends.

(1)

* Ajout des friends.

### 01/05

* Ajout des sessions.
* Ajout des jointures sur les pointeurs.
* Doc sous la forme de tableaux.
* MAJ sur Like/Média/Event

Dans la plupart des objets, il y a une colonne contenant une String {pointeur}, ceci correspond à un ID, qui va permettre de faire une liaison direct avec une autre row dans la DB. Permettant par la suite une jointure lors des récupérations des données.

