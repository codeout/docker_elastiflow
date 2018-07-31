FROM docker.elastic.co/logstash/logstash:6.3.2

EXPOSE 2055/udp 6343/udp

RUN bin/logstash-plugin install logstash-codec-sflow && \
    bin/logstash-plugin update logstash-codec-netflow logstash-input-udp logstash-filter-dns
