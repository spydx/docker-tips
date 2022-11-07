# MariaDB / Mysql

Most of these settings will work on MySQL databases also.

## Populating the database

To populate a MariaDB, you have to mount a folder with files to the `/docker-entrypoint-initdb.d` folder and specify the `MARIADB_DATABASE` variable.
This is then run on the first initialization of the container, importing all the data into the specified database defined in the environment variable `MARIADB_DATABASE`.
The files are run in alphabetical order, and with this in mind, you can organize how things are imported.

Supported filetypes:

- `.sh`
  A note about `.sh` files is that they are sourced if the execute flag is omitted on the file.
- `.sql`
- `.sql.gz`
- `.sql.xz`
- `.sql.zst`

Source:
[MariaDB@DockerHub](https://hub.docker.com/_/mariadb)
[MySQL@DockerHub](https://hub.docker.com/_/mysql)