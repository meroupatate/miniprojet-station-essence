# CSC5003: Web sémantique et infrastructures pour le big data

## Mini-projet - Exploration de données

### Présentation

Ce mini-projet utilise la base de données [Prix des carburants en France le 9 janvier 2021](https://www.data.gouv.fr/fr/datasets/r/087dfcbc-8119-4814-8412-d0a387fac561) issue de www.data.gouv.fr afin de réaliser l'objectif métier de suggérer à un automobiliste des stations essences correspondant à des critères qu'il aura sélectionnés (distance ou prix).

Afin d'enrichir ce jeu de données avec des informations sur la distance que l'utilisateur doit parcourir pour atteindre le point de vente de carburant, on utilisera l'API d'[openroute service](https://openrouteservice.org/).

### Dépendances
Le projet est effectué en Scala avec Apache Spark dans un notebook Jupyter. Il est nécessaire pour tester le notebook d'installer un noyau Scala pour Jupyter comme [almond](https://almond.sh/).

Il est également nécessaire de disposer d'un token `openroute service` qui peut être obtenu gratuitement en s'inscrivant [ici](https://openrouteservice.org/dev/#/signup).


### Démo
- Exemple d'un automobiliste situé à Palaiseau qui recherche un point de vente carburant:
[CSC5003_Mini-projet.md](CSC5003_Mini-projet.md)

- Exécuter le notebook soi même:
```bash
echo $YOUR_ORS_TOKEN > .ors_token
jupyter notebook CSC5003_Mini-projet.ipynb
```
