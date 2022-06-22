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

Now we have launched the grafana with docker we can go to:
```sh
http://localhost:3000
```

We have to introduce the user 'admin', pass 'admin' and do it again. Now we should reach to this page.

![Grafana first page](https://github.com/federicoperezmarina/101_grafana_first_steps/blob/main/img/grafana_first_page.png)
