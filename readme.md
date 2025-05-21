Create .env file and run:
```bash
curl -O https://raw.githubusercontent.com/yingkeen/n8n-pi/refs/heads/master/n8n-swarm.yml
set -a && source .env && set +a && envsubst < n8n-swarm.yml > new-n8n-swarm.yml
docker stack deploy -c new-n8n-swarm.yml n8n
```
