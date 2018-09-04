FROM alpine
RUN apk add openjdk8 openjdk8-jre openjdk8-jre-base \
&& wget https://sonatype-download.global.ssl.fastly.net/nexus/3/nexus-3.0.2-02-unix.tar.gz \
&& tar -xvf nexus-3.0.2-02-unix.tar.gz 

ENTRYPOINT /nexus-3.0.2-02/bin/nexus run
