# Huntweb NodeJS

Back-End application inspired by [Product Hunt](https://www.producthunt.com/) made with Node.js, Express and MongoDB

The purpose of this application is to practice the concepts of Node.js as seen in the [Rocketseat](https://rocketseat.com.br/) free course.

## Runing it localy

### Docker and MongoDB

This project needs a Mongo Database to work, it can be set up easily with [Docker](https://www.docker.com/products/docker-desktop)

After Docker installation run `docker pull mongo` to download a Mongo image

Then create a new container, and redirect ports with `docker run --name mongodb -p 27017:27017 -d mongo`

Now you can start your container when needed with `docker start mongodb`

### NPM / Yarn

Inside de project root directory run `npm install` or `yarn install` to install the project dependencies

Finally you can run `npm run dev` or `yarn dev` to start de back-end server

## Avaliable Routes

> You can easily test all te routes with [Insomnia](https://insomnia.rest/download/)

- GET http://localhost:3001/api/products
  - List all products (return products array)
  
- GET http://localhost:3001/api/products/:id
  - Show a expecific product (return a product)
  
- POST http://localhost:3001/api/products
  - Store a new product (return the new product)
  
- PUT http://localhost:3001/api/products/:id
  - Update a product (return the updated product)
  
- DELETE http://localhost:3001/api/products/:id
  - Delete a product (return an empty message)
  
## Directory Structure

- **node_modules** (project dependencies)
- **src** (main application files)
  - **controllers** (application controllers)
  - **models** (application models)
  - **routes** (application routes)
- **server** (initialize the application)
