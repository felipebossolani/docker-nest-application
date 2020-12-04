
# Nest.JS + Docker - Primeiro App

Olá esse é um projeto de estudos envolvendo Nest.js e Docker. A idéia é fazer um build simples para entender o funcionamento de ambos.
## Pré-Requisitos
* [Docker](https://www.docker.com/)
* [Node](https://nodejs.dev/)
* [Nest.js](https://nestjs.com/)

## Criando do zero
Caso queira criar do zero, execute os seguintes comandos:
```
npm install -g @nestjs/cli
nest new docker-nest-application
cd docker-nest-application
```

## Executando
Para executar o projeto sem o uso de docker faça o seguinte comando:
```
npm run start
```
Abre o browser e aponte para https://localhost:3000

## Dockerfile

O dockerfile foi feito para suportar variavel de ambiente no build ou não. Caso omita a variavel de ambiente então será "buildado" para produção.

## Execução do docker
Para o build da imagem:
```
docker build -t docker-nest-app
```
Para a execução da imagem:
```
docker run -p 3000:3000 docker-nest-app
```
Abre o browser e aponte para https://localhost:3000
