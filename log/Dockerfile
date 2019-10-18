FROM	goharbor/harbor-log:v1.9.0
COPY	./logrotate.conf /etc/logrotate.d/logrotate.conf
COPY	./rsyslog_docker.conf /etc/rsyslog.d/rsyslog_docker.conf
VOLUME	/var/log/docker/
EXPOSE	1514
CMD	["/bin/bash","/usr/local/bin/start.sh"]
