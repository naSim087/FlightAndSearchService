# welcome to flight setup

## project setup
  - clone the project on your local
  - execute `npm install` on the same paht as of your root directory
  - create a `.env` file in the root directory  and add the following 
    environment varaible
      - `PORT=3000`
  - inside the `src/config` folder create a new file `config.json` and the add the following piece of code 
    ```
       { "development": {
                        "username": "<your_db_login_name>",
                        "password": "<your_db_pass>",
                        "database": "Flights_Search_DB_DEV",
                        "host": "127.0.0.1",
                        "dialect": "mysql"
                        }
       }                


    ```
  - once you have added the db config as listed above then
   , go to the src folder from you terminal and then execute `npx sequelize db:create`




## DB design
  - Airplane table
  - Flight table
  - Airport table
  - city table

  - a flight belong to an airplane but one airplane can be used in multiple flights
  - a city has many airport but one airport belong to a only one city
  - one airport can have many flight, but a flight belongs to one airport
