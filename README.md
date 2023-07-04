"# php-7.4-symfony" 
# lancer le conteneur

docker compose up -d

# entrer dans le conteneur

docker exec -it www bash



# une fois dans le conteneur 
symfony new project --webapp
# vous devez avoir un dossier project 
cd project

# installer les dépendances qui manque de symfony
composer require doctrine/annotations

# aller sur le navigateur et taper l'url http://localhost:8000
# vous devez voir la page d'accueil de symfony
# aller sur le navigateur et taper l'url http://localhost:8081
# vous devez voir la page d'accueil de phpmyadmin
# aller sur le navigateur et taper l'url http://localhost:1080
# vous devez voir la page d'accueil de maildev
# pour arrêter le conteneur
docker compose down

