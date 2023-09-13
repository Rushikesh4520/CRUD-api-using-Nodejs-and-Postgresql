# CRUD-api-using-Nodejs-and-Postgresql

CRUD-api using Nodejs and Postgresql

Step1: Set Up Your Project
  1.create a new directory for your project and navigate into it:
    $mkdir nodejs-postgresql-crud
    $ cd nodejs-postgresql-crud
  2.Initialize your project with a 'package.json' file.
    $npm init -y

  Step2: Install Required Packages
    You'll need the 'express'. 'pg', and 'body-parser' packages in this application.
      $npm install express pg body-parser

  Step3: Set Up PostgreSQL
    Make sure you have Postgreql installed on your system. Create a new database and a table for this project.Here's an example  using the 'psql' command:
      $cd (postgresql bin path)
      $psql -U your_username (By default username is "postgres")
      CREATE DATABASE DATABASE-NAME;
      \.C DATABASE_NAME
      CREATE TABLE table_name (
          id SERIAL PRIMARY KEY,
          coloumn2 datatype,
          coloumn3 datatype
        );
        Example:
        CREATE DATABASE CRUD-APP;
      \.C crud_app
      CREATE TABLE users (
          id SERIAL PRIMARY KEY,
          username VARCHAR(255),
          email VARCHAR(255)
        );

  Step4: Create the Server
    Create a file named 'index.js' and set up your server:

  Step5: Start the Server
    $node index.js


Your CRUD application is now set up! You can use tools like Postman to test the API
endpoints('GET /users', 'POST /users', 'PUT /users/:id', 'DELETE /users/:id')
Remember to replace 'your_username' and 'your_password' with your actual
PostgreSQL credentials.
      
