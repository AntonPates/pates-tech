---
title: "Stop and remove all docker containers"
date: 2019-07-20T08:51:14+03:00
tags: ["docker", "remove container", "stop container"]
slug: "docker-stop-and-remove-containers"
description: "Stop and remove all containers"
---
Stop and remove all containers

```
$ docker stop $(docker ps -a -q)
$ docker rm $(docker ps -a -q)
```
<!--more-->

#### Links
[Docker stop](https://docs.docker.com/engine/reference/commandline/stop/), [Docker rm](https://docs.docker.com/engine/reference/commandline/rm/).