# MongoDB Starter

## Prerequisites

- Docker
- Docker Compose

## Usage

`data=<PATH> docker-compose up`

Example:

`data=./mydb docker-compose up`

This will save all the data in the local folder called `mydb`. If the folder does not exist it will create it.

<b>Attention</b>: the contents of the data folder is encrypted, using the database user-name and password. If you want to be able to do backups, uncomment the backup volume mapping inside the `docker-compose.yml` file, then set the environment variable.

By default, database user-name and password are both `root`, you can change this using th `db_user` and `db_password` environment variables, that you can set just like the `data` variable.
