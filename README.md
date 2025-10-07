# Final Assessment Projects

Step 1: Start Loki using Docker

docker run -d --name=loki -p 3100:3100 grafana/loki:2.9.0 \
  -config.file=/etc/loki/local-config.yaml

Step 2: Forward container logs to Loki using Promtail

docker run -d --name=promtail -v /var/log:/var/log \
  -v /var/lib/docker/containers:/var/lib/docker/containers:ro \
  -v /etc/promtail:/etc/promtail \
  grafana/promtail:2.9.0 \
  -config.file=/etc/promtail/promtail-docker-config.yaml

Step 3: Run a test container (example: hello-devops)

docker run --name hello-test hello-devops:latest

Step 4: View logs from Loki API (filtering by job name)

curl "http://localhost:3100/loki/api/v1/query?query={job=\"dockerlogs\"}"



✅ monitoring/loki_setup.txt
Step 1: Start Loki using Docker

docker run -d --name=loki -p 3100:3100 grafana/loki:2.9.0 \
  -config.file=/etc/loki/local-config.yaml

Step 2: Forward container logs to Loki using Promtail

docker run -d --name=promtail -v /var/log:/var/log \
  -v /var/lib/docker/containers:/var/lib/docker/containers:ro \
  -v /etc/promtail:/etc/promtail \
  grafana/promtail:2.9.0 \
  -config.file=/etc/promtail/promtail-docker-config.yaml

Step 3: Run a test container (example: hello-devops)

docker run --name hello-test hello-devops:latest

Step 4: View logs from Loki API (filtering by job name)

curl "http://localhost:3100/loki/api/v1/query?query={job=\"dockerlogs\"}"


✅ Add to README.md (Documentation Section)
## Monitoring with Loki

We use **Grafana Loki** to collect and query logs from Nomad jobs or Docker containers.

### Steps:
1. Start Loki:
   ```bash
   docker run -d --name=loki -p 3100:3100 grafana/loki:2.9.0 \
     -config.file=/etc/loki/local-config.yaml


Start Promtail to forward container logs:

docker run -d --name=promtail \
  -v /var/log:/var/log \
  -v /var/lib/docker/containers:/var/lib/docker/containers:ro \
  -v /etc/promtail:/etc/promtail \
  grafana/promtail:2.9.0 \
  -config.file=/etc/promtail/promtail-docker-config.yaml


Run a test container:

docker run --name hello-test hello-devops:latest


Query logs in Loki:

curl "http://localhost:3100/loki/api/v1/query?query={job=\"dockerlogs\"}"


Optionally, you can run Grafana to visualize logs:

docker run -d -p 3000:3000 grafana/grafana


Then connect Grafana to Loki (http://loki:3100) as a data source.


---

👉 Do you want me to also provide a **ready-made Promtail config file** (`promtail-docker-config.y

