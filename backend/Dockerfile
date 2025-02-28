# Utiliser une image Node.js comme base
FROM node:18

# Créer un répertoire de travail
WORKDIR /usr/src/app

# Copier le fichier package.json et package-lock.json (ou yarn.lock)
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier tous les fichiers du backend dans le container
COPY . .

# Exposer le port sur lequel le serveur tourne
EXPOSE 3000

# Démarrer le serveur (ou toute commande pour démarrer ton backend)
CMD [ "npm", "run", "start" ]
