FROM docker.io/anapsix/alpine-java
RUN apk add wget unzip
RUN wget http://download.jboss.org/wildfly/14.0.0.Final/wildfly-14.0.0.Final.zip
RUN unzip wildfly-14.0.0.Final.zip
RUN wget 'http://mirrors.jenkins.io/war-stable/latest/jenkins.war' -O '/wildfly-14.0.0.Final/standalone/deployments/jenkins.war'
ENTRYPOINT /wildfly-14.0.0.Final/bin/standalone.sh -b 0.0.0.0 -bmanagement 0.0.0.0

