# Hey I'm the /me route

-------------------------
## Effectuer une requête à l'API

Pour effectuer une requête à l'API il faut ajouter dans le header de chacune de vos requêtes :

`Authorization: Bearer ACCESS_TOKEN`

-------------------------
## /me -   Informations du profil 

```json
{
  "id": "54eb62cb998bc70c2463ab46",
  "provider": "google",
  "email": "address@gmail.com",
  "picture": "http://127.0.0.1:8080/media/avatars/54ecb78d5d9162d825c28cb7.min.jpeg",
  "name": "First Last",
  "first_name": "First",
  "last_name": "Last",
  "verified": true,
  "images": 2,
  "friends": 0,
  "badges": [
    {
      "name": "the name",
      "desc": "the desc",
      "title": "the title",
      "picture": "http://127.0.0.1:8080/media/badges/54fc86e391c284dc2153568a.jpeg"
    },
    ...
  ]
}
```