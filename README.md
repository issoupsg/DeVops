# Application Web CRUD avec API Utilisateur et Tests Intégrés

## Description

Ce projet consiste à créer une application web API utilisateur avec des fonctionnalités CRUD, stockant les données dans une base de données Redis. Le projet est enrichi par divers tests (unitaires, API, de configuration et de connexion) et inclut un point d'accès de vérification de l'état (health check) pour garantir le bon fonctionnement de l'application.

Cette application est basée sur un modèle de projet situé dans le dossier `courses/devops/modules/03.continuous-testing/lab`, avec des améliorations apportées à toutes les sections marquées "TODO".

## Fonctionnalités Implémentées

1. **API Utilisateur CRUD** : Création, lecture, mise à jour et suppression des utilisateurs via des requêtes HTTP.
2. **Stockage Redis** : Utilisation de Redis pour la gestion des données utilisateur.
3. **Tests** :
   - Tests unitaires pour vérifier les fonctions individuelles.
   - Tests API pour valider les requêtes HTTP.
   - Tests de configuration et de connexion pour garantir le bon fonctionnement de l'application dans différents environnements.
4. **Endpoint de vérification de l'état (Health Check)** : Un point d'accès dédié pour vérifier si l'application est opérationnelle.

## Captures d'Écran

Toutes les captures d'écran montrant l'application en action (interface utilisateur, ressources Kubernetes, etc.) sont disponibles dans le dossier `screenshots`.

- Exemple : ![Capture d'écran de l'interface API](./screenshots/api_interface.png)
- Exemple : ![Capture d'écran de Redis](./screenshots/redis_screen.png)

## Instructions d'Installation

### Pré-requis

- **Docker** : [Installer Docker](https://www.docker.com/get-started)
- **Redis** : [Installer Redis](https://redis.io/)
- **Node.js** (si vous utilisez Node.js) : [Installer Node.js](https://nodejs.org/)
- [Autres outils nécessaires selon votre choix de langage]

### Étapes d'Installation

1. Clonez ce dépôt :
   ```bash
   git clone https://github.com/votre-repo.git
