# Bergamo's DCNPM
> Docker Compose Nginx PHP MySQL

Ez LEMP Stack solution for Docker Compose that best fits my needs.

## Environment configuration
To deploy the application you have to define a couple of constants. Those are the name of the app and the root password of the DBMS.
You can do that by creating a `.env` file and adding those constants:
```.env
APP_NAME=<the application name>
MYSQL_ROOT_PASSWORD=<the password of the MySQL user>
```

To create a database on the application creation simply write all your SQL queries on `./config/init.sql` and the db will be initialized the first time you launch the application.
Note that if you you want to create a separate MySQL user (which is recommended for advanced security) you can do that in the `init.sql` file.

```sql
GRANT ALL PRIVILEGES ON <user>.* TO <database>@'%' IDENTIFIED BY <password>;
```

Forked from [stevenliebregt/docker-compose-lemp-stack](https://github.com/stevenliebregt/docker-compose-lemp-stack)