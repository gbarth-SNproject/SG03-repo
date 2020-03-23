FROM docker.elastic.co/beats/filebeat:7.6.0

RUN filebeat modules enable nginx
#RUN filebeat setup
RUN filebeat modules list

COPY /conf/filebeat.yml /usr/share/filebeat/filebeat.yml

USER root

#Create a directory to map volume with all nginx log files
RUN mkdir /usr/share/filebeat/nginxlogs

RUN chown -R root /usr/share/filebeat/
RUN chmod -R go-w /usr/share/filebeat/

