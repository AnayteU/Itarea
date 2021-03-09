FROM servergurus/ubuntu-jdk8
MAINTAINER Prasanjit Singh <nixgurus@gmail.com>

COPY wildfly-8.2.0.Final /opt/wildfly

COPY wildfly-spring-boot-sample-1.0.0.war /opt/wildfly/standalone/deployments/

RUN java -version

EXPOSE 8080 9990 9090

CMD ["/opt/wildfly/bin/standalone.sh", "-c", "standalone-full.xml", "-b", "0.0.0.0"]
