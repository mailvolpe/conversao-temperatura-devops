# Instalação e execução
- 1 - Clonar repositório forkeado do github.
- 2 - Instalar dependências do Node 'npm install'
- 3 - Testar com 'node server.js'
- 4 - Criar Dockerfile na pasta /src com setagem básica da imagem
- 5 - Buildar o container 'docker build -t mailvolpe/conversao-temperatura:v1 .'
- 6 - Rodar o container 'docker container run -d -p 8080:8080 mailvolpe/conversao-temperatura:v1'

# Boas práticas
- 7 - Setar a versão do node (Tag da imagem no comando 'FROM' do Dockerfile).
- 8 - Criar o .dockerignore e colocar o 'node_modules/' nele.

# Tags e Push 
- 9 - Fazer o push da v1 para o Docker Hub com 'docker push mailvolpe/conversao-temperatura:v1'
- 10 - Criar a tag latest com 'docker tag mailvolpe/conversao-temperatura:v1 mailvolpe/conversao-temperatura:latest'
- 11 - Fazer o push da latest para o Docker Hub com 'docker push mailvolpe/conversao-temperatura:latest'
- 12 - Apagar as imagens e rodar o container da V1 fazendo o Docker baixar a imagem do repositório Docker Hub
- 13 - Alterar um arquivo (View) para criar uma V2 com o comando 'docker build'
- 14 - Subir a V2 para o repositório com 'docker push'
- 15 - Definir a tag 'latest' para a imagem 'v2' com 'docker tag'
- 16 - Subir a imagem da latest para o Docker Hub (No vídeo 2:53:56, ele dá o comando para subir a v2 mas eu fiquei na dúvida com relação à isso porque a imagem criada foi a latest e a v2 já estava no repositorio)

# Teste final - Docker
- 17 - Rodar um container da V2 na porta 8081 para mostrar a execução simultanea dos dois containers
- 18 - Verificar as três imagens no Docker Hub (V1, V2, Latest)

# Kubernetes
- 19 - Rodando com Pod 'kubectl apply -f pod.yaml'
- 20 - Rodando com Replicaset 'kubectl apply -f replicaset.yaml'
- 21 - Rodando a aplicação em Kubernetes com 'kubectl apply -f deployment.yaml'