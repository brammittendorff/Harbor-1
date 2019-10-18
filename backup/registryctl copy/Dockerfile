FROM	goharbor/harbor-registryctl:v1.9.0
COPY	./registry/* /etc/registry/
COPY	./config.yml /etc/registryctl/config.yml
RUN	chown 10000:10000 -R /etc/registry/ && chown 10000:10000 -R /etc/registryctl/config.yml
ENV	CORE_SECRET=PDiS2gDJxvMtgW5q JOBSERVICE_SECRET=hsXbrV3GbxB573BM proxy_url=
VOLUME	/storage
