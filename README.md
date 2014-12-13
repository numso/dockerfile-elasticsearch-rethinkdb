# ElasticSearch/RethinkDB Dockerfile


This repository contains a Dockerfile which builds ElasticSearch and pre-installs the Head plugin and the RethinkDB river.


An [automated build](https://registry.hub.docker.com/u/numso/elasticsearch-rethinkdb/) for this repo is published to the public [Docker Hub Registry](https://registry.hub.docker.com/).


### Installation

1. Install [Docker](https://www.docker.com/).

2. Download the [automated build](https://registry.hub.docker.com/u/numso/elasticsearch-rethinkdb/) from the public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull numso/elasticsearch-rethinkdb`

   (alternatively, you can build an image from this Dockerfile: `docker build -t numso/elasticsearch-rethinkdb github.com/numso/dockerfile-elasticsearch-rethinkdb`)


### Usage

    docker run -it --rm -p 9200:9200 -p 9300:9300 numso/elasticsearch-rethinkdb
