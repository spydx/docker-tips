# Docker Tips

Collection of Docker tips

This repo is organized in the following way.
Under each folder, you will find a `docker-compose`
file that you can copy that will contain configuration for e.g a type of database.
E.g. in the folder `db` you will find `azure-edge` and `mariadb`

## Table of Content

- [Database]
  - [Azure-Edge](./db/docker-compose.azure-edge.md)
  - [Azure-Edge](./db/docker-compose.azure-edge.yml)
  - [MariaDB](./db/docker-compose.mariadb.md)
  - [MariaDB Example](./db/docker-compose.mariadb.yml)
- [Security](./security/)
  - [run-as-user](./security/RUN-USER.md)
  - [run-as-user Example](./security/Dockerfile.run-user)
- [Services]
  - [Depends-On](./services/docker-compose.depends_on.md)
  - [Depends-On Example](./services/docker-compose.depends_on.yml)