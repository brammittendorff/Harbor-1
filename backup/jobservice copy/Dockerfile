FROM	goharbor/harbor-jobservice:v1.9.0
COPY	./config.yml /etc/jobservice/config.yml
ENV	CORE_SECRET=PDiS2gDJxvMtgW5q JOBSERVICE_SECRET=hsXbrV3GbxB573BM CORE_URL=http://127.0.0.1:8081 JOBSERVICE_WEBHOOK_JOB_MAX_RETRY=10
ENV	HTTP_PROXY HTTPS_PROXY NO_PROXY=127.0.0.1,localhost,.local,.internal,log,db,redis,nginx,core,portal,postgresql,jobservice,registry,registryctl,clair
