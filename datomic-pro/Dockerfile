from dustinconrad/datomic-base

ENV DATOMIC_DATA $DATOMIC_HOME/data
ENV CONF_DIR /opt/datomic/conf
ENV CONF_FILENAME dev-transactor.properties

VOLUME $DATOMIC_DATA

EXPOSE 4334 4335 4336

CMD bin/transactor ${CONF_DIR}/${CONF_FILENAME}