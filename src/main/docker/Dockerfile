FROM jre

MAINTAINER Joscha Burkholz <joscha.burkholz@gmx.de.de>

ADD meetup-hello-world*exec.jar meetup-hello-world-app.jar

RUN bash -c 'touch /app.jar'

ENV JAVA_OPTS="$JAVA_OPTS -Djava.security.egd=file:/dev/./urandom"

ENTRYPOINT java $JAVA_OPTS -jar meetup-hello-world-app.jar
