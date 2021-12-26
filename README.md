# Docker compose file for PHP projects

## Settings for .env file

- WWW_DIR: base dir with PHP files 
- PORT: port on which the app should be exposed

## Database

It is expected that there exists a docker network `mariadb`. In this network a MariaDB instance must be accessible.
