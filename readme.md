1 - Clonar repositório forkeado do github.
2 - Instalar dependências do Node 'npm install'
3 - Testar com 'node server.js'
4 - Criar Dockerfile na pasta /src com setagem básica da imagem
5 - Buildar o container 'docker build -t mailvolpe/conversao-temperatura:v1 .'
6 - Rodar o container 'docker container run -d -p 8080:8080 mailvolpe/conversao-temperatura:v1'