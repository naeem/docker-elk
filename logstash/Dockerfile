ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash-oss:${ELK_VERSION}

COPY postgresql-42.1.1.jar /opt/logstash/postgresql-42.1.1.jar
RUN logstash-plugin install logstash-filter-jdbc
# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
