# Hey i'm the signup

Liste des informations nécessaires lors de l'inscription :

* Nom du provider utilisé (Google/Facebook)
* ID de l'utilisateur sur ce provider* (optional)
* Token utilisé pour accéder à l'API du provider*
* Nom du device
* ID de l'application (contenu dans la db)
* Secret de l'application (contenu dans la db)
* Unique ID du téléphone
* Nom du téléphone

> Ces info sont transmises par Google et Facebook lors de la connexion via le bouton "S'inscrire/Se connecter"

Envoyer une requête POST sur /signup contenant :	

* `auth_type=google/facebook`
* `access_token=TOKEN`
* `user_id=USER_ID` (optional)
* `client_id=CLIENT_ID`
* `client_secret=CLIENT_SECRET`
* `defive_id=DEVICE_ID`
* `device_name=DEVICE_NAME`

Un appel réussi à /signup renvoit un objet JSON :
```json
{
  "access_token": ".......",
  "expires_in": 600,
  "token_type": "Adok"
}
```

Les appels suivants à `/signup` reverra un nouvel objet JSON contenant les informations pour se connecter au service.