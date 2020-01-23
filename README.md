## Guacamole Setup

On initial setup, the mysql server needs to be started first, then all the other containers can start. This needs to be done in order to ensure, that the DB was initialized.

### Prestart

Make sure to setup the `*.env` files.

### First start

```shell
$ docker-compose up mysql
```

After MySQL has started all services, quit out of the container with `CTRL + C`.

After that you can start all services with:

```shell
$ docker-compose up
```

The guacamole service will be available after starting all services via `http://DOCKER-HOST-IP:8080/guacamole/`
