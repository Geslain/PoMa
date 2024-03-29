# 54q4r4

![Saqara Logo](https://cdn.jaimelesstartups.fr/wp-content/uploads/2021/09/Logo-Saqara-1500x535.jpg
"Saqara Logo")

## Description

54q4r4 Technical test. Please look into [api](api) and [client](client) for more information

## Install project

This project use the concept of [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). In order to clone the project and its submodules you have to use the following command:

```
git clone --recursive git@github.com:Geslain/54q4r4.git
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

## Test

You can import and use the [Postman](https://www.postman.com/) collection in [54q4r4.postman_collection.json](54q4r4.postman_collection.json) file
