# ELK STACK
- Elasticsearch (3 Nodes)
- Kibana
- Logstash


## Creating network
```
docker network create --driver overlay --attachable elastic
```

## Deploying Stack
```
docker stack deploy -c docker-compose.yml elkstack
```

## Remove Stack
```
docker stack rm elkstack
```

## Some important notes must be done before stack deploy
1. https://www.elastic.co/guide/en/elasticsearch/reference/current/vm-max-map-count.html

2. https://www.elastic.co/guide/en/elasticsearch/reference/current/setup-configuration-memory.html

