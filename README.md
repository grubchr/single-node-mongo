# single-node-mongo

Single node MongoDB docker container.

## Create a .env file

The .env file should contain the following:

```bash
MONGO_INITDB_ROOT_USERNAME=admin
MONGO_INITDB_ROOT_PASSWORD=password
ME_CONFIG_MONGODB_ADMINUSERNAME=admin
ME_CONFIG_MONGODB_ADMINPASSWORD=password
ME_CONFIG_BASICAUTH_USERNAME=admin
ME_CONFIG_BASICAUTH_PASSWORD=password
```

## Deploy

```bash
docker-compose up -d
```

Explicitly specify the .env file:

```bash
docker-compose --env-file .env up -d
```

## Shutdown

```bash
docker-compose down
```
