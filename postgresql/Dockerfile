FROM postgres:9.6.15-alpine

VOLUME /var/lib/postgresql/data


COPY ./docker-healthcheck.sh /docker-healthcheck.sh
COPY ./initial-notaryserver.sql /docker-entrypoint-initdb.d/
COPY ./initial-notarysigner.sql /docker-entrypoint-initdb.d/
COPY ./initial-registry.sql /docker-entrypoint-initdb.d/

ENV POSTGRESQL_HOST=127.0.0.1 POSTGRESQL_PORT=5432 POSTGRESQL_USERNAME=postgres POSTGRESQL_PASSWORD=root123 POSTGRESQL_DATABASE=registry POSTGRESQL_SSLMODE=disable

RUN chown -R postgres:postgres /docker-entrypoint.sh /docker-healthcheck.sh /docker-entrypoint-initdb.d \
    && chmod u+x /docker-entrypoint.sh /docker-healthcheck.sh 

ENTRYPOINT ["/docker-entrypoint.sh"]
HEALTHCHECK CMD ["/docker-healthcheck.sh"]
EXPOSE 5432
CMD ["postgres"]
