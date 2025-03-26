# Utilisation de Node.js
FROM node:17-alpine

# Définition du répertoire de travail
WORKDIR /app

# Vérification du contenu
RUN ls -la  # Ajout pour voir le contenu

# Copier package.json et package-lock.json
COPY package*.json ./

# Vérification après copie
RUN ls -la  # Vérifie si les fichiers sont bien copiés

# Installation des dépendances
RUN npm install

# Copier tout le projet
COPY . .

# Exposer le port
EXPOSE 3000

# Commande de lancement
CMD ["node", "index.js"]
