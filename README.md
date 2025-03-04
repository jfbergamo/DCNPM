# Bergamo's DCNPM
> Docker Compose Nginx PHP MySQL

Ez LEMP Stack solution for Docker Compose that best fits my needs.

## Environment configuration
To define the constants of the application create a `.env` file containing the following constats:
```
APP_NAME=<the application name>
MYSQL_USER=<the MySQL username that is going to connect to the db>
MYSQL_PASSWORD=<the password of the MySQL user>
```

To create a database on the application creation simply write all your SQL queries on `init.sql` and the db will be initialized the first time you launch the application.

Forked from [stevenliebregt/docker-compose-lemp-stack](https://github.com/stevenliebregt/docker-compose-lemp-stack)