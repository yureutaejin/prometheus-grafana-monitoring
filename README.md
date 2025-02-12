# (HomeLab Application) Prometheus-Grafana Monitoring

Application to monitor the metrics of the HomeLab infrastructure using Prometheus and Grafana.

Application is being deployed by [`Homelab-IaC`](https://github.com/yureutaejin/homelab-iac)

## Quick Start

1. Set configuration for each of components(`prometheus`, `grafana`, etc...)
   - `alertmanager` needs SLACK_WEBHOOK_URL which can not be directly set in `alertmanager.yml` file. You need to set `sed -i` command or `envsubst` command in your CD workflows separately.
2. Run `docker compose up -d` in the root directory of the repository
