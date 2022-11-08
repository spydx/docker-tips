# Depend On

Depend on is a nice way of orchestrating your services in the correct boot order.
This, unfortunately, does not do a health check validating that e.g. the database is up and alive before you launch your API.
There are methods for doing this, and in most cases this `depends_on:` will suffice enough to get your services up in the correct order.

## Example

[Depends_on](./docker-compose.depends_on.yml)

## Third-party tools

There are third-party tools to do this better.
You can find them here:

Sources:
[Docker Control Startup and Shutdown](https://docs.docker.com/compose/startup-order/)
