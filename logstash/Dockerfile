FROM docker.elastic.co/logstash/logstash:7.8.0

RUN logstash-plugin install logstash-input-http

COPY config/logstash.yml /usr/share/logstash/config/logstash.yml
COPY pipeline /usr/share/logstash/pipeline
