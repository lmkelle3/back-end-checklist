# back-end-checklist
## for a simple React project

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

### Setting up your back-end
1. If you have not already, install dbconfig globally (see https://github.com/johnazre/dbconfig)
 - npm install -global dbconfig
 - run dbconfig, this will walk you through creating a new project from scratch
 - delete views folder if not needed
 - configure the existing folders to match the data you will be using (i.e. delete "todos" and replace with "messages")
 
### You will need to install packages & dependencies (this will automatically create node modules)
1. run npm i express body-parser cors knex morgan

### You will need to create a .gitignore file in your project folder if you will be uploading to github
1. create .gitignore

### You will need to install nodemon globally if you wish to run your server using nodemon
1. npm install --global nodemon

### Begin creating your tables for your database
1. create migrations
 - knex migrate:make 01_table
1. create seeds
 - knex seeds:make 01_table
 
 * Pause to create your database *
 
 ### Create the database
 1. create new database in Postico using PostgreSql
 - select "+ Database"
 - then select "+ Table"
 - label your database and table with the same name as your data migrations database and table
 1. create your table to match your migrations data structure
 - do not include an "id" row for your data if you have table.increments() for your data
 
  * Resume working with your migrations/seeds *
 
 1. run seeds to populate your database in Postico
 - knex seeds:run 01_table
 1. create controllers
 1. create routes

## Test Your Routes
1. test with postman
- full CRUD testing
