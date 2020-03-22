# Build a blog using Nest.js, TypeScript, React, MongoDB and Auth0

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)

Guía práctica de [Auth0](https://auth0.com/blog/modern-full-stack-development-with-nestjs-react-typescript-and-mongodb-part-1).

## Backend API

### Instalar dependencias

```bash
cd blog-api
npm install
```

### Crear archivo .env

Luego de la instalación crear archivo `.env` de `.env.dist`:

```bash
cp .env.dist .env
```

Abrir y editar el archivo `.env` con sus propias credenciales

```
# MongoDB
DB_HOST=localhost
DB_PORT=27017
DB_NAME=nest-blog-project

# Auth
AUTH0_DOMAIN=YOUR_AUTH0_DOMAIN
AUTH0_AUDIENCE=http://localhost:5000/api
```

### Ejecutar la aplicación

En otra terminal ejecutar la aplicación con:

```bash
npm run start:dev
```

La api quedará disponible en `http://localhost:5000/`.

### Api Doc

Colección Postman en `blog-api/api-doc/nest-react-auth0-blog.postman_collection.json`

## Frontend

### Instalar dependecias

```bash
cd blog-frontend
npm install
```

### Crear archivo .env

Luego de la instalación crear archivo `.env` de `.env.dist`:

```bash
cp .env.dist .env
```

Abrir y editar el archivo `.env` con sus propias credenciales

```
# API
REACT_APP_SERVER_BASE_URL=http://localhost:5000

# Auth
REACT_APP_AUTH0_DOMAIN=YOUR_APP_AUTH0_DOMAIN
REACT_APP_AUTH0_CLIENT_ID=YOUR_APP_AUTH0_CLIENT
REACT_APP_AUTH0_AUDIENCE=http://localhost:5000/api
REACT_APP_AUTH0_REDIRECT_URI=http://localhost:3000
```

### Ejecutar la aplicación

```bash
npm start
```

### Test App

La aplicación quedará disponible en `http://localhost:3000`

## Prerequisitos

[Node.js](https://nodejs.org/en/), [Yarn package manager](https://yarnpkg.com/lang/en/docs/install/#mac-stable), [MongoDB](https://docs.mongodb.com/v3.2/installation/), [TypeScript](https://www.typescriptlang.org/) y [Auth0](https://manage.auth0.com/dashboard)

## Built With

[Nest.js]()
[React.js]()
[Auth0]()
[TypeScript]()
[MongoDB]()
