FROM centos

RUN yum install -y sudo && sudo yum -y update \
    && sudo yum install -y golang nginx wget unzip glibc.i686 && cd /opt/ && sudo wget https://dl.gogs.io/0.11.53/gogs_0.11.53_linux_amd64.zip \
    && sudo unzip gogs_0.11.53_linux_amd64.zip
WORKDIR /opt/gogs/
ENTRYPOINT ./gogs web -port 10000

