FROM node:16.15.1
WORKDIR /app

#Esse fica acima para executar o 'npm install' quando alterar um dos arquivo packege*.json
COPY ./package*.json ./

RUN npm install

#Esse fica abaixo para que não seja preciso executar o 'npm install' quando alterar um arquivo
COPY . .

EXPOSE 8080
CMD ["node", "server.js"]