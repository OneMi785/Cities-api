# Documentation de l'API REST - Base Nationale des Villes Françaises

Bienvenue dans la documentation de l'API REST pour accéder à la Base Nationale des Villes Françaises. Cette API vous permet de récupérer des informations sur les villes françaises, y compris le nom de la ville, le code postal, la longitude, et l'altitude.

## Accès à la Base Nationale des Villes Françaises

Cette API vous donne accès à la base nationale des villes françaises. Vous pouvez effectuer des requêtes pour obtenir des informations sur les villes spécifiques ou pour récupérer une liste complète de toutes les villes.

## Méthodes d'accès

L'API dispose de deux méthodes d'accès :

### GET (Collection)

La méthode GET (collection) vous permet d'obtenir la liste complète des villes françaises.

- Endpoint : `GET` https://127.0.0.1:8000/api/cities
- Description : Récupère la liste complète des villes françaises.

## Exemple d'utilisation :

Les réponses de l'API sont au format JSON et contiennent des informations sur les villes, y compris les attributs suivants :
- `id` : L'identifiant unique de la ville.
- `name` : Le nom de la ville.
- `zip` : Le code postal de la ville.
- `lon` : La longitude de la ville.
- `lat` : L'altitude de la ville.

Voici un exemple de réponse JSON pour la méthode GET (Élément) :

```json
[
  {
    "id": 1,
    "name": "Paris",
    "zip": "75000",
    "lon": 2.3522,
    "lat": 48.8566
  }
  {
    "id": 2,
    "name": "Marseille",
    "zip": "13000",
    "lon": 5.3698,
    "lat": 43.2965
  },
  // ... (autres villes)
]
```

### GET (Élément)

La méthode GET (élément) vous permet d'obtenir les détails d'une ville spécifique en utilisant son identifiant.

- Endpoint : `GET` https://127.0.0.1:8000/api/cities/{id}
- Description : Récupère les détails d'une ville spécifique en utilisant son identifiant.
- Exemple d'utilisation :

## Exemple d'utilisation :

Voici un exemple de réponse JSON pour la méthode GET (Élément) :

```json
{
"id": 1,
"name": "Paris",
"zip": "75000",
"lon": 2.3522,
"lat": 48.8566"
}