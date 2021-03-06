# Vuesplash

This is a sample application using Laravel, Vue, Vue Router and Vuex.

## Requirement

- [Docker](https://www.docker.com/)
  - docker-compose

## Usage

Run server:

```console
$ docker-compose up
```

Go to `http://localhost` and you'll see the website.

## Install

Clone repository:

```console
$ git clone https://github.com/PiroHiroPiro/vuesplash.git
$ cd vuesplash
```

Copy env files:

```console
$ cp ./docker/php/.env.example ./docker/php/.env
$ cp ./docker/mysql/.env.example ./docker/mysql/.env
$ cp ./src/vuesplash/.env.example ./src/vuesplash/.env
```

Enter the database name, root password, username, password, aws access key, aws secret key and aws bucket name in the copied env files `./docker/php/.env`, `./docker/mysql/.env` and `./src/vuesplash/.env`:

Build images:

```console
$ docker network create vuesplash_network
$ docker-compose build
```

Install packages:

```console
$ docker-compose run php npm install
/src# cd /src/vuesplash
/src/vuesplash# npm install
```
