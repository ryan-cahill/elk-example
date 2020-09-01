FROM docker.elastic.co/elasticsearch/elasticsearch:7.8.0

# TODO: use in initContainer
RUN sysctl -w vm.max_map_count=262144

COPY ./elasticsearch.yml /usr/share/elasticsearch/config/elasticsearch.yml

# template.spec.securityContext.fsGroup = 1000 in elasticsearch deployment is REQUIRED
