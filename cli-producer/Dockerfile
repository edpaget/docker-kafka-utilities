# DOCKER-VERSION 1.2.0
# VERSION 0.2

FROM zooniverse/kafka
MAINTAINER Edward Paget <ed@zooniverse.org>

RUN echo "#!/bin/bash \n ./opt/kafka_$SCALA_VERSION-$KAFKA_VERSION/bin/kafka-console-producer.sh \$@" > /usr/local/bin/kafka-producer && \
    chmod +x /usr/local/bin/kafka-producer

ENTRYPOINT ["kafka-producer"]
