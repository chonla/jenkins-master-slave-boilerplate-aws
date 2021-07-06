# Jenkins Master/Slave Boilerplate

## Setup

1. Set plugins you want to use in `./dockers/main/plugins.txt`. Plugins `swarm` is mandatory.
2. Run `JENKINS_USERNAME=<jenkins-username> JENKINS_PASSWORD=<jenkins-password> docker-compose up -d` to start Jenkins.
3. Run `docker-compose restart` to make sure Jenkins loads all newly installed plugins.

## Running Jenkins with insecure docker registries

Add the follow option to `docker:dind` key.

```
    command: ["--insecure-registry=<registry-host-1>:<registry-host-1-port>", "--insecure-registry=<registry-host-2>:<registry-host-2-port>"]
```
