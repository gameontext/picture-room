FROM websphere-liberty:latest

MAINTAINER Ben Smith

ADD https://download.elastic.co/logstash-forwarder/binaries/logstash-forwarder_linux_amd64 /opt/forwarder
ADD ./servers/gameon-pictureroom /opt/ibm/wlp/usr/servers/defaultServer/

COPY ./forwarder.conf /opt/forwarder.conf
COPY ./startup.sh /opt/startup.sh

EXPOSE 9080

CMD ["/opt/startup.sh"]
