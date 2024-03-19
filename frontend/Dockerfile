# Utilisez une image de base contenant Node.js
FROM node:16

# Définissez le répertoire de travail dans le conteneur
WORKDIR /home/vagrant/projet_mern/frontend

# Copiez les fichiers du frontend dans le conteneur
COPY . .

# Installez les dépendances
RUN npm install

# Construisez l'application
RUN npm run build

# Exposez le port sur lequel le serveur frontend s'exécute
EXPOSE 3000

# Commande pour démarrer le serveur frontend
CMD ["npm", "start"]

