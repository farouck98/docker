# Définir l'image de base
FROM node:14-alpine

# Création de l'utilisateur non-root
RUN adduser -D mohamedfarouck

# Définition de l'utilisateur non-root
USER mohamedfarouck

# Définition du répertoire de travail
WORKDIR /app

# Copie du fichier package.json
COPY package.json /app/package.json
RUN npm install

# Copie du reste de l'application
COPY . .

# Exposition du port 3000
EXPOSE 3000

CMD ["npm", "start"]

