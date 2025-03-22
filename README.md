# 
Le fichier README.md doit contenir des instructions claires pour exécuter le projet.

# Projet DevOps : Serveur HTTP Minimaliste avec Docker

Ce projet met en place un serveur HTTP minimaliste en Python, conteneurisé avec Docker.

## Structure du projet
- `app/server.py` : Code du serveur HTTP.
- `dockerfile` : Fichier pour construire l'image Docker.
- `docker-compose.yml` : Fichier pour orchestrer le déploiement avec Docker Compose.

## Instructions pour exécuter le projet
## Partie 1
1. creer le fichier server.py:Le fichier server.py contient le code d'un serveur HTTP minimaliste en Python utilisant le module http.serve
2. creer le fichier dockerfile:Le fichier dockerfile permet de construire une image Docker contenant l'application.
3. creer le fichier docker_compose.yml:Le fichier docker-compose.yml permet de simplifier le déploiement du projet avec Docker Compose.
4. creer le fichier readme pour expliquer les instructions pour executer le projet

## Partie B

### Sans Docker Compose
1. Construire l'image Docker :
   ```bash
   docker build -t mon_server .
2. Exécuter le conteneur : docker run -p 8000:8000 mon_server pour que le serveur sera accessible à l'adresse http://localhost:8000
avec docker compose :docker-compose up
3. Taguer l'image Docker: docker tag mon_server abibatou77/mon_server:v1.0
Taguer l'image pour qu'elle soit prête à être poussée sur DockerHub.
4. Se connecter à DockerHub : docker login 
Pousser l'image sur DockerHub: docker push abibatou77/mon_server:v1.0
et maintenant sera disponible sur dockerhub sous le nom abibatou77/mon_server:v1.0


