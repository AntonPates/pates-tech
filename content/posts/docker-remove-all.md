---
title: "Remove all unused containers, networks and images."
date: 2019-07-20T08:50:14+03:00
tags: ["docker", "remove", "prune", "image", "container", "network"]
slug: "docker-remove-all"
description: "Remove all unused containers, networks, images both dangling and unreferenced."
---
Remove all unused containers, networks, images both dangling (not associated with a container) and unreferenced.

```
$ docker system prune
```
<!--more-->
Remove all unused images not just dangling ones.
```
$ docker system prune -a
```

To prune volumes use `--volumes` option.
#### Links
[Docker docs](https://docs.docker.com/engine/reference/commandline/system_prune/), [digitalocean](https://www.digitalocean.com/community/tutorials/how-to-remove-docker-images-containers-and-volumes).