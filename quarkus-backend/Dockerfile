FROM quay.io/quarkus/centos-quarkus-maven:20.0.0-java8 as quarkus-dev
COPY --chown=1001:1001 . /quarkus-backend
WORKDIR /quarkus-backend
RUN env && \
    mvn package && \
    mvn dependency:go-offline -Dnative