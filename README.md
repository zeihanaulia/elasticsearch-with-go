# Elasticsearch with go

## Install Elasticsearch

Sumber: [https://hub.docker.com/_/elasticsearch](https://hub.docker.com/_/elasticsearch)

```bash
docker network create elasticnw
```

```bash
docker run -d --name elasticsearch --net elasticnw -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" elasticsearch:7.9.3
```