1 - Clonar repositório forkeado do github.
2 - Instalar dependências do Node 'npm install'
3 - Testar com 'node server.js'
4 - Criar Dockerfile na pasta /src com setagem básica da imagem
5 - Buildar o container 'docker build -t mailvolpe/conversao-temperatura:v1 .'
6 - Rodar o container 'docker container run -d -p 8080:8080 mailvolpe/conversao-temperatura:v1'

# Boas práticas

7 - Setar a versão do node (Tag da imagem no comando 'FROM' do Dockerfile).
8 - Criar o .dockerignore e colocar o 'node_modules/' nele.
9 - Fazer o push da v1 para o Docker Hub com 'docker push mailvolpe/conversao-temperatura:v1'
10 - Criar a tag latest com 'docker tag mailvolpe/conversao-temperatura:v1 mailvolpe/conversao-temperatura:latest'
11 - Fazer o push da latest para o Docker Hub com 'docker push mailvolpe/conversao-temperatura:latest'

12 - Apagar as imagens e rodar o container da V1 fazendo o Docker baixar a imagem do repositório Docker Hub
13 - Alterar um arquivo (View) para criar uma V2
