# Les villes

Voici le listing de toute les fonctions cloud disponible pour les city.

Le schéma complet du json à envoyer aux fonctions cloud:

| Nom de la variable | Type attendu                 | Description|
| ------------------ | ---------------------------- | ------ |
 name | String | Nom de la ville
 nbWizz | Number | Compteur de wizz pour la ville

nbWizz est incrémenté à la création de wizz par rapport a la ville renseignée.

----------------------
## checkAddress
----------------------

*Retourne la liste des adresses qui match la recherche*

Paramètres:

* q
