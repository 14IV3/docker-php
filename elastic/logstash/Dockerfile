FROM docker.elastic.co/logstash/logstash:5.5.2
RUN rm -f /usr/share/logstash/pipeline/logstash.conf
USER root
RUN chown -R logstash:root /usr/share/logstash/config; \ 
    chmod 0750 /usr/share/logstash/config;

USER logstash
ADD ./pipeline/logstash.conf /usr/share/logstash/pipeline/
ADD ./config/logstash.yml /usr/share/logstash/config/
