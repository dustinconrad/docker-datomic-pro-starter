from dustinconrad/docker-oracle-java8

ENV DATOMIC_VERSION 0.9.5173
ENV DATOMIC_HOME /opt/datomic-pro-${DATOMIC_VERSION}

ADD .mydatomic /etc/wgetrc

RUN apt-get --quiet update \
  && apt-get --quiet --yes install unzip \
  && wget -q https://my.datomic.com/repo/com/datomic/datomic-pro/${DATOMIC_VERSION}/datomic-pro-${DATOMIC_VERSION}.zip -O /tmp/datomic.zip \
  && unzip /tmp/datomic.zip -d /opt \
  && rm -f /tmp/datomic.zip \
  && rm /etc/wgetrc

WORKDIR $DATOMIC_HOME