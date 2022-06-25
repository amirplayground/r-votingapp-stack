Steps:
1. Deploy PODs
    - redis as "redis"
    - postgres as "db"
    - worker-app as "worker"
    - voting-app as "vote"
    - result-app as "result"
2. Enable Connectivity (create ClusterIP)
    - redis-service
    - postgres-service
3. External Access (create NodePort)
    - voting-app-service
    - result-app-service


IMAGES LEGEND
redis - redis
postgres - postgres
voting-app - kodecloud/examplevotingapp_vote:v1
result-app - kodecloud/examplevotingapp_result:v1
worker-app - kodecloud/examplevotingapp_worker:v1