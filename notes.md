# How to build

* The container tag in the docker-compose.yml file should be set to the OHDSI WebAPI release number.
* The Dockerfile WEBAPI_WAR argument should be set to the WebAPI version for the required WebAPI release.
* The Dockerfile WEBAPI_RELEASE environment variable should be set to the WebAPI release number.

```
docker-compose build broadsea-webtools

# How to run the container

Edit the docker-compose.yml file to specify the database connection info and Docker host IP/port
See <https://github.com/OHDSI/Broadsea> for more information.

```
docker-compose up -d

# How to stop and remove the container

```
docker-compose down