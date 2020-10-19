# AdGuard Docker Settings

AdGuard with Docker enables you to rewrite your DNS settings for ease-of-use for services such as [stonehenge](https://github.com/druidfi/stonehenge).

## Requirements

You need to have these applications installed to operate on all environments:

- [Docker](https://github.com/druidfi/guidelines/blob/master/docs/docker.md)

## Get started

```
$ git clone git@github.com:shamalainen/adguard-docker.git
```

After cloning the repo, change into the directory and start the docker container

```
$ cd adguard-docker
$ docker-compose up -d
```

## Credentials

Logging into AdGuard is possible at http://localhost:8053/
- Username: `admin`
- Password: `admin`

## Pre-configured filters

This repo already has a pre-configured custom DNS response for [stonehenge](https://github.com/druidfi/stonehenge).
- `*.docker.sh` => `127.0.0.1`
