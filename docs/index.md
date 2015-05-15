# Sommaire

* [`Accueil` - Cette page.](index.md)
* [`User` - Les utilisateurs](user.md)
* [`Friend` - Les amis](friend.md)
* [`N_Friend` - Les notifications d'amis](n_friend.md)
* [`Session` - Les sessions](session.md)
* [`Comment` - Les commentaires](comment.md)
* [`Event` - Les moments](event.md)
* [`Like` - Les j'aimes/gemmes](like.md)
* [`Media` - Les médias](media.md)
* [`Participant` - Les participants](participant.md)
* [`Error Codes` - Les code d'erreurs](error.md)


## MAJ de la doc

### 15/05

* Ajout de la fonction EventGetByCity
* Ajout du champ city dans Event (string)

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

---------
## Accueil

Documentation de l'api wizzEM

Voir la documentation de [Parse](http://www.parse.com) selon le SDK sur lequel vous travaillez.

Pour pouvoir utiliser l'api, au lieu de faire des requêtes sur une route, vous avez simplement à appeler la **fonction cloud** que vous désirez utiliser.

Une fonction cloud est une fonction qui est stocké chez parse, et qui peux être appelé depuis n'importe quel SDK.

Voir la documentation de votre SDK chez parse pour savoir comment appeler une fonction cloud.

<img src="../images/doc_cloudfunc.jpeg" alt="Doc" style="width: 800px;"/>

