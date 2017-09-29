---
layout: post
title:  "Docker入门二"
categories: Docker
tags: Docker primer
author: Edward
---

* content
{:toc}

简单讲一下docker中的service，官方解释：In a distributed application, different pieces of the app are called “services.”。





## docker-compose.yml

用于define, run, and scale一个service

```yml
version: "3"
services:
  web:
    # replace username/repo:tag with your name and image details
    image: username/repository:tag
    deploy:
      replicas: 5
      resources:
        limits:
          cpus: "0.1"
          memory: 50M
      restart_policy:
        condition: on-failure
    ports:
      - "80:80"
    networks:
      - webnet
networks:
  webnet:
```