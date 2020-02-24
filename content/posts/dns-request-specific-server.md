---
title: "Query a specific DNS Server with dig"
date: 2020-02-24T21:30:14+03:00
tags: ["dig", "DNS", "request", "cloudflare", "resource record", "query", "question", "answer"]
slug: "dns-query-specific-server"
description: "Query a specific DNS Server with dig"
---
Query Cloudflare (1.1.1.1) for pates.tech with dig.

```
$ dig pates.tech @1.1.1.1
```

<!--more-->

```
$ dig pates.tech @1.1.1.1

; <<>> DiG 9.10.6 <<>> pates.tech @1.1.1.1
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 32244
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 1452
;; QUESTION SECTION:
;pates.tech.			IN	A

;; ANSWER SECTION:
pates.tech.		600	IN	A	104.198.14.52

;; Query time: 85 msec
;; SERVER: 1.1.1.1#53(1.1.1.1)
;; WHEN: Mon Feb 24 23:01:12 +03 2020
;; MSG SIZE  rcvd: 55
```

## In the ANSWER SECTION
```
;; ANSWER SECTION:
pates.tech.		600	IN	A	104.198.14.52
```
- pates.tech. - an owner name (FQDN - Fully Qualified Domain Name) , i.e., the name of the node to which this resource record pertains.
- 600 - TTL (Time To Live), a 32 bit signed integer that specifies the time interval that the resource record may be cached before the source of the information should again be consulted.  Zero values are interpreted to mean that the resource record can only be used for the transaction in progress, and should not be cached.
- IN stands for Internet in CLASS field.
- A is type of the resource record.
- 104.198.14.52 - for A-type records IPv4-string that describes the resource.




#### Links
[RFC 1035](https://tools.ietf.org/html/rfc1035).
