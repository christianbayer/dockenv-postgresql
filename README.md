# PostgreSQL + pgAdmin 4 | Docker environment


## Quick Start
* Clone or download the repository
* Run `copy .env.example .env` and set up your environment configuration (see default values below)
* Run `docker-compose up -d`


## Environment
The .env file has the following configurations available, with their default values:
* `POSTGRES_TAG`: Version of PostgreSQL image. Default value is `latest`
* `PGADMIN_TAG`: Version of pgAdmin image. Default value is `latest`
* `POSTGRES_USER`: PostgreSQL default user. Default value is `postgres`
* `POSTGRES_PASSWORD`: PostgreSQL default password. Default value is `postgres`
* `PGADMIN_PORT`: pgAdmin port. Default value is `5050`
* `PGADMIN_USER`: pgAdmin default email. Default value is `pgadmin4@pgadmin.org`
* `PGADMIN_PASSWORD`: pgAdmin default password. Default value is `admin`


## Access to PostgreSQL: 
* `localhost:5432`
* **Username:** defined in `POSTGRES_USER`, by default `postgres`
* **Password:** defined in `POSTGRES_PASSWORD`, by default `postgres`


## Access to pgAdmin: 
* Access `http://localhost:5050` with the following credentials:
* **Username:** defined in `PGADMIN_USER`, by default `pgadmin4@pgadmin.org`
* **Password:** defined in `PGADMIN_PASSWORD`, by default `admin`


## Add a new server in PgAdmin:
* **Host name/address**: `postgres`
* **Port**: `5432`
* **Username**: defined in `POSTGRES_USER`, by default: `postgres`
* **Password**: defined in `POSTGRES_PASSWORD`, by default `postgres`