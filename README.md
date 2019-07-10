# NodeJS Quickstart

Project quickstart with NodeJS, Babel, Express and Docker. 

By leveraging the power of Docker you don't need to install Node JS in your computer. You just run everything from a Docker container.

Babel makes it possible to use the newest Javascript features available in ECMAScript.  

## Requirements

- Git;
- Docker;
- Docker Compose.

## Installation

1) Clone the repository:

```
git clone git@github.com:fernandohu/quickstart-nodejs-express-babel.git
```

2) Use Docker to run `npm install` on the NodeJS source code at `app/` folder:

```
docker-compose run --rm node npm install
```

3) Run `docker compose` to start up the development environment:

```
docker-compose up
```

After running `docker-compose up` the application should be accessible at http://localhost:3000.

Try the following API Requests (GET):

- http://localhost:3000/messages/
- http://localhost:3000/messages/1
- http://localhost:3000/messages/2
- http://localhost:3000/users
- http://localhost:3000/users/1
- http://localhost:3000/users/2
- http://localhost:3000/session

## Developing

The source code resides at `/app`. 

## Executing npm 

You can execute `npm` commands by calling the `node` service:

```
docker-compose run -rm node npm XXX
```

The commands will be always executed in the `app` folder.

## Connect to the container

```
docker exec -it nodejs bash
```
