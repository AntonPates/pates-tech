---
title: "Go web application security checklist"
date: 2019-08-25T08:50:14+03:00
tags: ["security checklist", "golang","web application security" ,"Natalie Pistunovich"]
slug: "app-security-checklist"
description: "Application security checklist"
---

Checklist based on video of [@NataliePis](https://twitter.com/nataliepis) from GoWayFest 3.0 in Minsk.

[Data](/posts/app-security-checklist#data) | [Code](/posts/app-security-checklist#code) | [Dependencies](/posts/app-security-checklist#dependencies)

<!--more-->
### Data {#data}
+ Passwords;
+ User Data;
+ Secrets management.

### Code {#code}
+ Input validation;
+ SQL injection;
+ Static code analysis: https://github.com/securego/gosec;
+ Endpoints for debug;
+ Logging and monitoring.

### Dependencies {#dependencies}
+ List of direct and indirect dependencies: go.mod;
+ Analysis of direct and indirect dependencies: goreportcard.com maybe helpful;
+ Reproducible builds: go modules;
+ Deps blacklist with https://github.com/OpenPeeDeeP/depguard.




{{< youtube HEKbmb_FHrQ >}}