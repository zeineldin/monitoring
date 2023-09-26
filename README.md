## ( Docker / Host ) Monitoring with cAdvisor,Node-Exporter using Prometheus and Grafana

--------


![prom2](https://user-images.githubusercontent.com/20526165/82630796-10899900-9bf4-11ea-8815-5a373c604b6c.png)


--------

## Definitions : 

1. [Prometheus](https://prometheus.io/): is a time series database used for monitoring.

2. [Grafana](https://grafana.com) : GUI or Frontend for Prometheus.

3. [cAdvisor](https://github.com/google/cadvisor): is an open-source tool developed by Google to monitor containers. It can collect, aggregate, process, and export container-based metrics  such as CPU and memory usage, filesystem, and network statistics. 

4. [[Node exporter](https://github.com/prometheus/node_exporter)  : is an open-source time-series monitoring and alerting system for cloud-native environments, including Kubernetes, hosted by the (CNCF), and we are going to use it to monitor the hosted machine. 


## Grafana Dashboard used :

1. Node Exporter ( ID: 1860 )

2. Docker Host & Container Overview ( ID:395 )

3. Docker monitoring with node selection (ID: 8321)

      [you can find more dashboards here](https://grafana.com/grafana/dashboards) 


## Monitoring Client

### Cadvisor, Node Exporter

Please note to configure the Firewall "allow cadvisor and Node-Exporter ports and IPS between server and client"


## Monitoring Server 
### Prometheus, Grafana 


1. Firewall "allow cadvisor and Node-Exporter ports and IPS for the machine you want to see the dashboard"
     ``` - targets: ['<ip>:<port>','<ip>:<port>']```
