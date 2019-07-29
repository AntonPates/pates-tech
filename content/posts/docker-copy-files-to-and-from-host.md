---
title: "Copy file from container to host and vice versa"
date: 2019-07-30T01:51:14+03:00
tags: ["docker", "copy file from container", "copy file to container"]
slug: "docker-copy-files-to-and-from-host"
description: "Copy file from container to host and vice versa"
---
To copy file from container to host

```
$ docker cp [CONTAINER_NAME|CONTAINER_ID]:/path/to/file/in/container /host/destination/path
```
<!--more-->
To copy file from host to container

```
$ docker cp /host/destination/path [CONTAINER_NAME|CONTAINER_ID]:/path/to/file/in/container
```

#### Links
[Docker cp](https://docs.docker.com/engine/reference/commandline/cp/).