# Hey  I'm the login page !

Envoyer une requête POST sur `/login` contenant :

1. Dans le header
	* `Authorization: Adok STRING` où STRING représente la chaine obtenu via /signup
2. Dans le body
	* `grant_type=adok`

Un appel réussi à `/login` renvois un objet formé comme suit :
```json
{
  "access_token": "2d10b4c018c90b95503aeba737dd569843252a43fdae45fb4089439aca88b0e1",
  "refresh_token": "36bde2d2099ece0b25d9bd2c70633b9cbace232e1ccfa898c0a891bf243e3c19",
  "expires_in": 3600,
  "token_type": "Bearer"
}
```

1. `access_token` : contient le token permettant d'accéder à l'API
2. `refresh_token` : contient un token servant à générer un nouveau Token et invalider l'ancien (renvoi de nouveau un objet json)
3. `expires_in` : Nombre de secondes avant que le token n'expire.
4. `token_type` : Type de token

-------------------------
### Effectuer une requête à l'API

Pour effectuer une requête à l'API il faut ajouter dans le header de chacune de vos requêtes :

`Authorization: Bearer ACCESS_TOKEN`

-------------------------
### Refresh Token

Pour générer un nouveau token, vous devez envoyer une requête POST sur `/login` avec :

1. Dans le header
	* `Authorization: Basic CHAINE_BASE64` où CHAINE_BASE64 doit être générer comme suite base64encode(client_id+':'+client_secret)
2. Dans le body
	* `grant_type=refresh_token`
	* `refresh_token=REFRESH_TOKEN`

Si l'appel se passe correctement, un nouvel objet json est renvoyé.
