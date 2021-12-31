
# Configure vim prometheus/prometheus.yml
```
# A scrape configuration containing exactly one endpoint to scrape:
# Here it's Prometheus itself.
scrape_configs:
  # The job name is added as a label `job=<job_name>` to any timeseries scraped from this config.

  - job_name: 'containeradvisor'
    # Override the global default and scrape targets from this job every 5 seconds.
    scrape_interval: 5s
    static_configs:

            # - targets: ['cadvisor:8080']
      - targets: ['cadvisor:8080'] # -->  cadvisor is the container name and the internal port "8080"


  - job_name: 'node-exporter'
    # Override the global default and scrape targets from this job every 5 seconds.
    scrape_interval: 5s
    static_configs:

            #  - targets: ['nodeexporter:9100']
      - targets: ['nodeexporter:9100'] #--> nodeexporter is the container name and the internal port 

```
