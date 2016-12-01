1. `docker-compose build`
2. `docker-compose up`
3. login to [grafana](http://localhost:3000) (admin:admin)
4. setup data source: `http://<elastic-container-ip>:9200`
  - have to use elasticsearch container IP, as the hostname won't work
  - find IP with `docker inspect grafanaelasticsearch_elasticsearch_1 | grep IPAddress`
