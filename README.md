## Setting file

----
### [ .dockerignore & .gitignore ]
The Docker ignore file informs your Docker builds of which files to not include while the Git ignore does the same for your Git commits

### [ .env ]
This provides information to Docker Compose that is essential for our application but should never be stored in version control

## Server

----
We’ll be building this Express server across 3 files: index.js, routes/routes.js, and models/Document.js. Express.js is a minimalist Node.js web framework that utilizes the concept of middleware. As a request comes into the server it flows through each middleware in order until it either hits the end and errors out or a function does some computation based on it and returns. Let’s start off with index.js