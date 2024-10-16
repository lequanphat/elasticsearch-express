## Build Elasticsearch and Kibana with Docker

### Step 1: Run docker compose:

```bash
docker-compose up
```

### Step 2: Access Elasticsearch container:

```bash 
docker exec -it elasticsearch /bin/bash
```

### Step 3: Create Elasticsearch service token:

```bash
bin/elasticsearch-service-tokens create elastic/kibana default
```

### Step 4: Replace ELASTICSEARCH_SERVICE_TOKEN by your token, then run docker compose:

```bash
docker-compose up
```

Navigate to http://localhost:5601 in your browser to access Kibana.