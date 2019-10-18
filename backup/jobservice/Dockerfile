FROM goharbor/harbor-jobservice:v1.9.0

ADD ./config.yml /etc/jobservice/config.yml

ENV CORE_SECRET=PvGTaXZ0dI4U5efj
ENV JOBSERVICE_SECRET=dZMbXPrQC72qvzOA
ENV CORE_URL=http://core:8080
ENV JOBSERVICE_WEBHOOK_JOB_MAX_RETRY=10
ENV HTTP_PROXY=
ENV HTTPS_PROXY=
ENV NO_PROXY=127.0.0.1,localhost,.local,.internal,log,db,redis,nginx,core,portal,postgresql,jobservice,registry,registryctl,clair


VOLUME /var/log/jobs

EXPOSE 8083