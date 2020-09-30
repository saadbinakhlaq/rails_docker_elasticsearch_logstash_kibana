# Integrate Rails logs with Elasticsearch, Logstash, and Kibana in Docker Compose

# Installation

```
$ docker-compose build
$ docker-compose run rails bundle rake db:create
$ docker-compose run rails bundle exec db:schema:load
```

Running the server

```
$ docker-compose up
```

# Simulate Requests
docker exec -it docker-rails-elasticsearch-logstash-kibana_rails_1 rake simulate:traffic

# Check kibana
open "http://localhost:5601"
When opening for the first time add index as `logstash-*` and then you can view all the logs

