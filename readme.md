# Task Manager REST API
This is a back-end code repository.This is a full featured Task Management REST API back-end built with Javascript,Node.js,MongoDB and Heroku.
- Application endpoint : https://stuli-task-manager-api.herokuapp.com/

 ## Features include:

- Pagination and filtering of server responses to avoid slow page load times.
- Full CRUD features for User and Task instances.
- Hash encryption of passwords and access management with JWT tokens.  
- Restricted user access to CRUD operations based on JWT tokens.
- Upload of User Profile Picture in JPEG/PNG/JPG formats.

### SETUP INSTRUCTIONS

Node.js and npm (Latest version) must be installed on your machine.  In terminal type the following commands:
```
git clone https://github.com/sachtuli/task-manager-api.git
cd task-manger-api
sudo npm install
mkdir config
cd config
touch dev.env
vi dev.env
```

Insert the following lines in `dev.env`, replacing all `<content>` with your own information:

```
PORT=<port number>
MONGODB_URL=<mongodb connection string>
JWT_SECRET=<unique key of your choice to generate JSON web tokens>
```

To run the web server return to the root of the repository and type:
```
npm run dev
```
Alternatively you may name `config/prod.env` or `config/staging.env` and appropriately run the web server with `npm run prod` or `npm run staging`.

### Deployment
- This App is deployed on [Heroku](https://www.heroku.com/). You can sign up for free-tier and deploy the application. 
- Steps can be found here [Getting Started on Heroku with Node.js](https://devcenter.heroku.com/articles/getting-started-with-nodejs).
- For Deployment on Heroku, MongoDB Cluster is required. You can set up a free-tier one here. [MongoDB](https://www.mongodb.com/atlas/database)

### API USAGE
All HTTP requests can be made from software such as [Postman](www.getpostman.com). Postman is free and exists for all major operating systems.

