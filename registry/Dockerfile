FROM goharbor/registry-photon:v2.7.1-patch-2819-v1.9.0

ADD ./config.yml /etc/registry/
ADD ./ /etc/registry/root.crt
VOLUME /storage
#VOLUME /etc/registry

EXPOSE 5000
