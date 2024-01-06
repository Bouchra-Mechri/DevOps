# Utilisez l'image Python Alpine officielle comme image de base
FROM python:alpine

# Définit le répertoire de travail à l'intérieur du conteneur
WORKDIR /usr/src/app

# Copie le fichier requirements.txt dans le répertoire de travail
COPY requirements.txt /usr/src/app

# Installe les dépendances Python spécifiées dans requirements.txt
#no cache bch my3mlch save lel cache 3la image
RUN pip install --no-cache-dir -r requirements.txt

# Copie l'ensemble du projet dans le répertoire de travail du conteneur
COPY . /usr/src/app

#8000 howa port fi wst image bch y5dm wst conteneur 
# Spécifie la commande pour exécuter le serveur de développement Django
CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]

#bch njm nchouf application mt3i m machine 
# Expose le port 8000 pour permettre les connexions externes
EXPOSE 8000
