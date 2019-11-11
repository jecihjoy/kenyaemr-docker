# Openmrs platform docker
This a docker image for kenya emr distribution
It contains everything needed to run kenya emr. Enable users to get started without having to setup the distrution themselves
It includes the runtime environment, modules, war file, and the required docker files.
Rename the main.env.example to main.env and configure

DB_NAME=db_name
OPENMRS_DB_USER=db_user
OPENMRS_DB_PASS=db_pass
OPENMRS_MYSQL_HOST=db_host
OPENMRS_MYSQL_PORT=db_port

to the correct database.

Ensure you have docker and docker compose installed correctly

Run  docker build -t 10.50.80.56:5005/kenyaemr:updated . to create the docker image

Run docker-compose up  to run the docker image

Head over to http://localhost:8080/openmrs  
