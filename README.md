# prometheus_node_exporter

Deploy Prometheus Node Exporter for monitoring machine metrics such as CPU, memory, disk usage, and more.

```bash
   curl -fsSL https://get.docker.com -o get-docker.sh
   sudo sh get-docker.sh
```

```bash
   git clone https://github.com/A-nony-mous/prometheus_node_exporter
   cd prometheus_node_exporter
   docker compose up -d
```

Add config to prometheus.yml:

```yml
  - job_name: 'JOB_NAME'
    static_configs:
      - targets: ['JOB_NAME:9100']
```

To get public ip, use

```bash
   curl ip.sb
```
