# Monitoring & Logging Stack: Prometheus + Grafana + Loki

This repo provides a production-style **observability** lab using Docker Compose:
- **Prometheus** for metrics
- **Node Exporter** (host metrics)
- **cAdvisor** (container metrics)
- **Grafana** dashboards
- **Loki + Promtail** for logs

## Quick Start
```bash
docker compose up -d
```

Then open:
- Grafana: http://localhost:3000  (default login: admin / admin)
- Prometheus: http://localhost:9090

## What to show
- Prometheus scrape configs + service discovery basics
- Dashboarding in Grafana
- Alert rules (example included)
- Log pipeline: Promtail → Loki → Grafana Explore

## Repo Structure
- `docker-compose.yml`
- `prometheus/` scrape config + alert rules
- `loki/` Loki config
- `promtail/` Promtail config
- `grafana/` provisioning (datasources + dashboards)
- `dashboards/` JSON dashboards

---

**Author:** Manthan Panchal  
**GitHub:** https://github.com/manthannovember95-pixel
