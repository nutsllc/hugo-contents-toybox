---
title: "Quick Start"
date: 2018-12-29T11:02:05+06:00
weight: 2
---

### STEP1: Installation

Clone the toybox-proxy repository.

```
$ cd /path/to/clone
$ git clone https://github.com/nutsllc/toybox-proxy.git
```

### STEP2: Settings

Copy ``path/to/toybox-proxy/bin/.env.example`` to the same directory as ``.env``.
Edit ``.env`` file.  example below.


```bash
vi .env

PROXY_HOME=/path/to/toybox-proxy
TOYBOX_UID=1000
TOYBOX_GID=1000

PROXY_CACHE=true
```

### STEP3: Run Containers

#### Start Proxy Container
```bash
$ cd tobox-proxy/bin
$ docker-compose up -d
```

It will start three containers. Nginx, docker-gen and letsencrypt-nginx-proxy-companion container.

* Nginx: Proxy Server
* docker-gen: Generate nginx conf files dynamically.
* letsencrypt-nginx-proxy-companion: create and update TLS cirtifications.


