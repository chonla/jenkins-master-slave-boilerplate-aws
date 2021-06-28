FROM jenkinsci/blueocean:latest

WORKDIR /opt
ADD ./plugins.txt .

RUN echo "<------ Install Jenkins Plugins"
RUN jenkins-plugin-cli -f /opt/plugins.txt

WORKDIR /var/jenkins_home/init.groovy.d
ADD ./bypass.groovy .

EXPOSE 80
EXPOSE 50000