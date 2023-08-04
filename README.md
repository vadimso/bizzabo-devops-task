 Instructions
 
 1-create webhook in slack and put it in alertmanager config map file
 
 2-define slack channel to receive the alerts
 
 3- install each component (prometheus, alertmnager,grafana,hello-world-app ) as deployment on kubernetes via kubectl apply (the service is a loadbalancer type in order to access from outside)
 
 4- add in /etc/prometheus alerts file in following location (file exists in prometheus folder) /etc/prometheus/alert.rules.yml
 
5 - create a datasource for prometheus in grafana (look for grafana-datasource-config.yaml file ) via kubectl

6- set grafana dashboard for getting  non 200 ok from hello-wolrd app 
