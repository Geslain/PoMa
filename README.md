# PoMa

![logo.png](logo.png)

PoMa is a project management tool. PoMa simply stand for PrOject MAnagment.


## Description

PoMa project management tool. Please look into [api](api) and [client](client) for more information

## Install project

This project use the concept of [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). In order to clone the project and its submodules you have to use the following command:

```
git clone --recursive git@github.com:Geslain/poma.git
```

## Start project

* First create a `.env` file. Environment variables are listed in `.env.template` file.

```
cp .env.template .env
```

* (Optional) Install [docker](https://docs.docker.com/engine/install/) and [docker compose](https://docs.docker.com/compose/install/)
* Launch docker compose
```
docker compose up
```
* (Optional but funnier) Load database archive for seeds data
```shell
source .env
docker exec poma-mongo-1 sh -c "exec mongorestore --uri='mongodb://${DATABASE_USER}:${DATABASE_PASSWORD}@127.0.0.1:27017'  --archive=./all-collections.archive"
```

All seeded users passwords are: `test`

## Test

You can import and use the [Postman](https://www.postman.com/) collection in [poma.postman_collection.json](poma.postman_collection.json) file
