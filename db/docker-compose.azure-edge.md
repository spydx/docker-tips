# Azure Edge

## MSSQL_PACKAGE=/backup

This setting allows us to create a custom folder where we can place a database backup in the form of a `DACPAC` or `BACPAC` to be auto-imported when we first time initializes the docker container.
This relives some work when importing a clean database, e.g. you can do `docker-compose rm` and `docker-compose up` and you will have a brand clean database restored from the `DACPAC` or `BACPAC`.

You can further, in the commented-out section specify the datalocations so you can have direct access to the database if needed.

## Sources

[Configure Azure Edge Sql using Environment variables](https://learn.microsoft.com/en-us/azure/azure-sql-edge/configure#configure-by-using-environment-variables)