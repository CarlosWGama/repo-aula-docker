# Passo a Passo para criar uma imagem e disponibilizar no servidor

1 - Crie sua conta no site do [Docker Hub](https://hub.docker.com/)
2 - Crie um Repositório novo [link](https://hub.docker.com/repository/create)
3 - Crie um arquivo Dockerfile com suas regras 
4 - Crie a imagem com o comando build onde o nome da imagem deve ser igual ao do repositório
```
    #Comando:
    docker image build -t nome-imagem caminho-dockerfile
    
    #Exemplo
    docker image build -t carloswgama/aula-docker:latest .
```
5 - Logue no docker hub pelo terminal com o comando ``` docker login ```
6 - Envie a sua imagem com o comando push
```
    #Comando:
    docker image push nome-image-igual-nome-repositorio
    
    #Exemplo
    docker image push carloswgama/aula-docker 
```

