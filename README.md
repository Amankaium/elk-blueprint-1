# elk-blueprint

Deploy a usable ELK setup in minutes.

Usages:

1. At deployment time, 2 port mappings are being set. Example case would be:
   * 5601->80 for Kibana: elk-kibana.envs.subutai.cloud
   * 9200->9200 for ElasticSearch: elk-es.envs.subutai.cloud:9200
2. Double check the port mapping status after the environment's creation
3. When the BP is correctly provisioned, feed some data to ElasticSearch:
   This is mostly sending JSON data using POST request to it, a complete example
   can be found at 
   https://www.elastic.co/guide/en/kibana/6.3/tutorial-load-dataset.html
4. Since we have populated some data into ES, find it in Kibana:
   * Open Kibana in web browser (in our case http://elk-kibana.envs.subutai.cloud)
   * Start your customization!

