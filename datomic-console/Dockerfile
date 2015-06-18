from dustinconrad/datomic-base

ENV DATOMIC_ALIAS dev
ENV DATOMIC_URL datomic:dev://datomic-db:4334/

EXPOSE 8989

CMD bin/console -p 8989 ${DATOMIC_ALIAS} ${DATOMIC_URL}