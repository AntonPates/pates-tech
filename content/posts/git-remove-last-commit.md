---
title: "Git remove last commit"
date: 2019-08-14T08:50:14+03:00
tags: ["git", "reset hard", "remove commit"]
slug: "git-remove-last-commit"
description: "Git remove last commit"
---
Remove last commit.

```
$ git reset --hard HEAD^
```
<!--more-->
To remove two last commits for example
```
$ git reset --hard HEAD~2
```



#### Links
[Git reset](https://git-scm.com/docs/git-reset).