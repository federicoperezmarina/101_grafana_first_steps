# 101_grafana_first_steps
This repository to learn about grafana dashboarding &amp; alerting

## Table of Contents
* [Grafana in a Docker container](#grafana-in-a-docker-contanier)

## Grafana in a Docker container
First of all we are going to install grafana in a docker container to show how it works

```sh
$ docker volume create grafana-storage
$ docker run -d --name=grafana -p 3000:3000  \
    -v grafana-storage:/var/lib/grafana \
    grafana/grafana
```