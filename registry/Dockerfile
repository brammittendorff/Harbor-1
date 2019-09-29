FROM goharbor/registry-photon:v2.7.1-patch-2819-v1.9.0

#ADD ./config.yml /etc/registry/
ADD ./ /etc/registry/root.crt
ADD ./install_cert.sh  /harbor
ADD ./docker-entrypoint.sh /docker-entrypoint.sh
RUN chmod +x /harbor/install_cert.sh \
&& chmod u+x /docker-entrypoint.sh

#VOLUME /storage
#VOLUME /etc/registry

EXPOSE 5000

ENTRYPOINT ["/docker-entrypoint.sh"]


