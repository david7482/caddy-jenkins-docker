# caddy-jenkins-docker
Setup Jenkins with Caddy as https proxy in Docker

## Requirement
- Install  [docker](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/) and [docker-compose](https://docs.docker.com/compose/install/#prerequisites) first
- Make sure the uid and gid of current login user are both 1000 (jenkins docker's requirement)

## How to run
```
$ cd ~
$ git clone https://github.com/david7482/caddy-jenkins-docker.git
$ cd caddy-jenkins-docker

**In Caddyfile, modify 'jenkins.example.com' to your jenkins domain**

$ DOCKERGID=`getent group docker | awk -F: '{print $3}'` docker-compose up -d
```
