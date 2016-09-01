# sails-js

## Getting Started
1. install sails globally with npm
    ```
    sudo npm -g install sails
    ```

2. create new sails app
    ```
    npm install -g sails-js
    ```

3. start the server
    ```
    cd sails-js
    sails lift
    ```

4. app is ready and running at:
    http://localhost:1337/

## Install dependencies
1. project dependencies package.json
    ```
    npm install
    ```

2. front-end dependencies with bower
    1. init bower
        ```
        cd assets
        bower init
        ```
    2. describe dependencies bower.json
    3. install dependencies
        ```
        bower install
        ```
    4. configure pipeline.js
        1. add bower css to load
        2. add bower js to load

## Connect to DB
1. Install DB driver
    ```
    npm install sails-mysql --save
    ```
2. Config connection at config/connection.js
    ```
    mysql: {
           adapter: 'sails-mysql',
           host: 'YOUR_MYSQL_SERVER_HOSTNAME_OR_IP_ADDRESS',
           user: 'YOUR_MYSQL_USER',
           password: 'YOUR_MYSQL_PASSWORD',
           database: 'YOUR_MYSQL_DB'
     },
    ```
3. Config default connection at config/models.js
    ```
    connection: 'someMysqlServer',
    migrate: 'alter'
    ```
4. Install ORM driver
    ```
    npm install waterline --save 
    ```

## Create a REST API
1. Generate
    ```
    sails generate api User
    ```
2. api/controllers/UserController.js
3. api/models/User.js
http://iliketomatoes.com/implement-passport-js-authentication-with-sails-js-0-10-2/
