# Integrate Rails logs with Elasticsearch, Logstash, and Kibana in Docker Compose

# Simulate Requests
docker exec -it docker-rails-elasticsearch-logstash-kibana_rails_1 rake simulate:traffic

# Check kibana
open "http://localhost:5601"
When opening for the first time add index as `logstash-*` and then you can view all the logs

