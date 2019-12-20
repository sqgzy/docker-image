FROM ssresearch/maven:openjdk8-openj9

#COPY simplelogger.properties $MAVEN_HOME/conf/logging/simplelogger.properties
ENV VERSION "17.03.1-ce"
RUN curl -L -o /tmp/docker-$VERSION.tgz https://download.docker.com/linux/static/stable/x86_64/docker-$VERSION.tgz \
    && tar -xz -C /tmp -f /tmp/docker-$VERSION.tgz \
    && mv /tmp/docker/docker /usr/bin \
    && rm -rf /tmp/docker-$VERSION /tmp/docker
