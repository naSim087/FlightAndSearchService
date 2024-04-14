# welcome to flight setup

## project setup
  - clone the project on your local
  - execute `npm install` on the same paht as of your root directory
  - create a `.env` file in the root directory  and add the following 
    environment varaible
      - `PORT=3000`
  - inside the `src/config` folder create a new file `config.json` and the add the following piece of code 
    ---
        "development": {
                        "username": "<your_db_login_name>",
                        "password": "<your_db_pass>",
                        "database": "Flights_Search_DB_DEV",
                        "host": "127.0.0.1",
                        "dialect": "mysql"
                        }


    ---