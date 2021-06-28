# Jenkins Master/Slave Boilerplate

## Setup

1. Set plugins you want to use in `./dockers/main/plugins.txt`. Plugins `swarm` is mandatory.
2. Run `JENKINS_USERNAME=<jenkins-username> JENKINS_PASSWORD=<jenkins-password> docker-compose up -d` to start jenkins.