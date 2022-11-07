# MariaDB / Mysql

Most of these settings will work on MySQL databases also.

## Populating the database

To populate a MariaDB, you have to mount a folder with files to the `/docker-entrypoint-initdb.d` folder.
This is then run on the first initialization of the container.
The files are run in alphabetical order, and with this in mind, you can organize how things are imported.


When a container is started for the first time, a new database with the specified name will be created and initialized with the provided configuration variables. Furthermore, it will execute files with extensions .sh, .sql, .sql.gz, .sql.xz and .sql.zst that are found in /docker-entrypoint-initdb.d. Files will be executed in alphabetical order. .sh files without file execute permission are sourced rather than executed. You can easily populate your mariadb services by mounting a SQL dump into that directory and provide custom images with contributed data. SQL files will be imported by default to the database specified by the MARIADB_DATABASE / MYSQL_DATABASE variable.

Source:
[MariaDB@DockerHub](https://hub.docker.com/_/mariadb)
[MySQL@DockerHub](https://hub.docker.com/_/mysql)