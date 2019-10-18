FROM	goharbor/registry-photon:v2.7.1-patch-2819-v1.9.0
COPY	./registry/* /etc/registry/
COPY	./root.crt /etc/registry/root.crt
RUN	chown 10000:10000 -R /etc/registry
VOLUME	/storage
