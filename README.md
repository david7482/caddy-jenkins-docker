# caddy-jenkins-docker
Host Jenkins with Caddy as https proxy in Docker

## How to run
```
$ export DOCKERGID=`getent group docker | awk -F: '{printf "%d", $3}'`
$ docker-compose up -d
```
