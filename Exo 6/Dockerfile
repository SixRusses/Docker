# Utilise l'image officielle Node.js comme base
FROM node:14

# Définis le répertoire de travail dans le conteneur
WORKDIR /app

# Copie le fichier package.json et package-lock.json dans le conteneur
COPY package*.json ./

# Installe les dépendances
RUN npm install

# Copie le fichier db.sql dans le conteneur
COPY db.sql /docker-entrypoint-initdb.d/

# Copie le reste des fichiers dans le conteneur
COPY . .

# Expose le port 3000 pour l'application Node.js
EXPOSE 3000

# Commande pour démarrer l'application
CMD ["npm", "start"]
