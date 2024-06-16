FROM node:14-alpine
# Installation de Bash

RUN adduser -D mohamedfarouck
USER mohamedfarouck
WORKDIR /app
COPY package.json /app/package.json
RUN npm install
COPY . .

EXPOSE 4000
CMD ["npm", "start"]