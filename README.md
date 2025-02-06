Application Web avec React, Flask et MySQL
📌 Aperçu du Projet
Ce projet est une application web simple construite avec :

Frontend : React (Vite)
Backend : Flask (Python)
Base de données : MySQL
Conteneurisation : Docker & Docker Compose
📂 Structure du Projet
/web-app
│── /frontend (Application React)
│   ├── /public
│   ├── /src
│   │   ├── /components
│   │   ├── /pages
│   │   ├── App.js
│   │   ├── index.js
│   ├── package.json
│   ├── vite.config.js
│   ├── Dockerfile
│
│── /backend (API Flask)
│   ├── /app
│   │   ├── /routes
│   │   │   ├── user_routes.py
│   │   ├── /models
│   │   │   ├── user_model.py
│   │   ├── __init__.py
│   │   ├── main.py
│   ├── requirements.txt
│   ├── Dockerfile
│
│── /db (Initialisation de la Base de Données)
│   ├── init.sql
│
│── docker-compose.yml (Orchestration des Conteneurs)
│── README.md (Documentation)
🚀 Installation & Configuration
1️⃣ Prérequis
Assurez-vous d'avoir installé :

Docker
Docker Compose
2️⃣ Étapes d'Installation
Cloner le dépôt
git clone https://github.com/your-repo/web-app.git
cd web-app
Construire et démarrer les conteneurs
docker-compose up --build
Arrêter les conteneurs
docker-compose down
🔧 Variables d'Environnement
Utilisez un fichier .env pour stocker les données sensibles :

DB_USER=root
DB_PASSWORD=password
DB_NAME=mydatabase
DB_HOST=db
🔒 Sécurisation
Utilisation des variables d’environnement pour les mots de passe et les informations sensibles.
Limitation des permissions et restriction des ports exposés pour renforcer la sécurité.
Utilisation du framework open-source OWASP Dependency-Check pour analyser les dépendances et détecter les vulnérabilités.
Mise en place de Fail2Ban pour limiter les tentatives de connexion infructueuses.
Activation de CORS et CSRF Protection avec Flask pour prévenir les attaques de type cross-site scripting.
🏗️ Points d'API (Flask)
GET /users → Récupérer tous les utilisateurs
POST /users → Créer un nouvel utilisateur
🎨 Frontend
Le frontend est construit avec React et Vite.
Les appels API sont effectués vers le backend Flask.
🗄️ Base de Données (MySQL)
Le fichier init.sql configure le schéma de la base de données.
MySQL est exécuté en tant que conteneur Docker.
📜 Licence
Ce projet est sous licence MIT.
