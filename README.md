# DevOps Project - User API with Redis

## Project Overview

**Deadline:** December 31, 2024
Ce projet est une application Web axée sur DevOps basée sur les laboratoires réalisés pendant le cours. Le projet couvre l'intégralité du cycle de vie DevOps, du développement au déploiement, en passant par la conteneurisation, l'orchestration et la surveillance. Les principaux composants comprennent :

- Une application API utilisateur avec fonctionnalité CRUD.
- Intégration de la base de données Redis pour le stockage.
- Différents niveaux de tests, y compris les tests unitaires, API, de configuration et de connexion.
- Point de terminaison de contrôle de santé pour garantir que l'application est fonctionnelle.


## Fonctionnalités Implémentées

1. **API utilisateur avec opérations CRUD** : l'application permet la création, la lecture, la mise à jour et la suppression d'utilisateurs, stockés dans une base de données Redis.
2. **Health Check Endpoint** : un point de terminaison dédié qui vérifie l'état de santé de l'application.
3. **Tests complets** :
    - Tests unitaires pour les fonctions individuelles.
    - Tests API pour la vérification des points finaux.
    - Tests de configuration et de connexion pour assurer une bonne intégration avec Redis.
4. **Pipeline CI/CD** : implémenté à l'aide de plates-formes telles que GitHub Actions ou GitLab CI/CD, permettant des tests, une création et un déploiement automatisés.
5. **Docker et Kubernetes** : l'application est conteneurisée avec Docker, orchestrée à l'aide de Docker Compose et déployée avec Kubernetes.
6. **Surveillance** : Prometheus et Grafana sont intégrés au cluster Kubernetes pour la surveillance et les alertes en temps réel.

## Captures d'Écran

Toutes les captures d'écran montrant l'application en action (interface utilisateur, ressources Kubernetes, etc.) sont disponibles dans le dossier `screenshots`.

- Exemple : ![Capture d'écran de l'interface API](./screenshots/api_interface.png)
- Exemple : ![Capture d'écran de Redis](./screenshots/redis_screen.png)

## Instructions d'Installation

Installation/configuration de l'environnement
1. Cloner ce dépôt :
   ```bash
   git clone https://github.com/your-repo/devops-project.git
   cd devops-project
   
2. Installer les dépendances :
   ```bash
   pip install -r requirements.txt

3. VM Vagrant Configuration :
- installer Vagrant et Ansible.
- Lancer le VM :
   ```bash
   Vagrant VM Setup
- Provisionnez la VM avec les playbooks Ansible :
   ```bash
   ansible-playbook playbooks/setup.yml

Exécutez l'application :
1. Docker
- Construire l'image Docker
    ```bash
    docker build -t userapi
- lancer le Docker container :
    ```bash
    docker run -p 5000:5000 userapi
    
2. Docker Composer
- lancer les services :
    ```bash
    docker-compose up
- Accédez à l'API sur http://localhost:5000

3. Kubernetes
- Commencer Minikube :
    ```bash
    minikube start
- Appliquez les manifestes Kubernetes :
    ```bash
    kubectl apply -f k8s/deployment.yaml

- Vérifier les services :
    ```bash
    kubectl get services

3. Tester l'Application












### Pré-requis

- **Docker** : [Installer Docker](https://www.docker.com/get-started)
- **Redis** : [Installer Redis](https://redis.io/)
- **Node.js** (si vous utilisez Node.js) : [Installer Node.js](https://nodejs.org/)
- [Autres outils nécessaires selon votre choix de langage]
