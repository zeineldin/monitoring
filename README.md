
# Monitoring Client
# Cadvisor, Node Exporter

you have to check 

1. Firewall "allow cadvisor and Node-Exporter ports and ips between server and client"


# Monitoring Server 
# Prometheus, Grafana 


1. Firewall "allow cadvisor and Node-Exporter ports and ips for the machine you want to see the dashboard"
     ``` - targets: ['<ip>:<port>','<ip>:<port>']```
