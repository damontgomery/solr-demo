# Setup

## Install Docker

[https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop)

## Start

```bash
docker compose up -d
```

## View the admin interface

Visit [http://localhost:8983/](http://localhost:8983/)

### View core

Select `Core Selector` > `Demo`

#### View field / query parsing

Go to `Analysis`

#### Try a search

Go to `Query`

#### View configuration

Go to `Files`

## To log into the Docker container

```bash
docker compose exec solr bash
```

### Some key folders

- `/var/solr/data` : Core configuration
- `/opt/docker-solr/scripts` : Scripts like the demo setup script

## To close

```bash
docker down
```

## More information on the Docker container

- [https://github.com/docker-solr/docker-solr](https://github.com/docker-solr/docker-solr)
- [https://hub.docker.com/_/solr](https://hub.docker.com/_/solr)

## This repository

This docker compose file was taken from the repository listed above and the demo script was added instead of the other setup scripts.
