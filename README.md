# back-end-checklist

1. Servers
1. Databases
1. Middleware



webpack
joi
knex
db config
express
body parser
cors
morgan? (comes with dbconfig)
node
nodemon
potgresql
postman
pg? (comes with dbconfig)
cookie-parser? (comes with dbconfig)
ejs? (comes with dbconfig)


## Node
### You will want to create a package.json wherever you are creating a new project.
1. npm init -y
 - initializes package.json
 
### You will need to install packages & dependencies (this will automatically create node modules)
1. npm i express
1. npm i body-parser
1. npm i cors
1. npm i knex

### You will need to create a .gitignore file in your project folder if you will be uploading to github
1. create .gitignore

### You will need to install nodemon globally if you wish to run your server using nodemon
1. npm install --global nodemon

### Create the server
1. If you have not already, install dbconfig globally (see https://github.com/johnazre/dbconfig)
 - npm install -global dbconfig
 - run dbconfig, this will walk you through creating a new project from scratch
 - install node modules:
  > express, knex, body-parser, cors, pg
 - delete views folder if not needed
1. create migrations
 - knex migrate:make 01_table
 - create controllers for 
