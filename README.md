# caddy-jenkins-docker
Setup Jenkins with Caddy as https proxy in Docker

## How to run
```
$ git clone https://github.com/david7482/caddy-jenkins-docker.git
$ cd caddy-jenkins-docker

**Modify Jenkins URL in Caddyfile**

$ export DOCKERGID=`getent group docker | awk -F: '{printf "%d", $3}'`
$ docker-compose up -d
```
