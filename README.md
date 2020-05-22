# ( Docker / Host ) Monitoring with cAdvisor,Node-Exporter & Prometheus and Grafana




![prom2](https://user-images.githubusercontent.com/20526165/82630796-10899900-9bf4-11ea-8815-5a373c604b6c.png)


--------

# Monitoring Client
## Cadvisor, Node Exporter

you have to check 

1. Firewall "allow cadvisor and Node-Exporter ports and ips between server and client"


# Monitoring Server 
## Prometheus, Grafana 


1. Firewall "allow cadvisor and Node-Exporter ports and ips for the machine you want to see the dashboard"
     ``` - targets: ['<ip>:<port>','<ip>:<port>']```
