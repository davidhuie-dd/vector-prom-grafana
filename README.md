# vector-prom-grafana

This repo showcases how to wire up Vector with Prometheus and Grafana.

# How to use

```
$ docker-compose up
```

# Available metrics

- host metrics (from the Vector host_metrics source)
- Datadog agent metrics (requires a local Datadog agent)

# Exported services

- Grafana: `localhost:3000`
- Vector (Datadog Agent interface): `localhost:9000`
- Prometheus: `localhost:9090`

# Configuring Grafana

1. Head to `localhost:3000`
1. Add the prometheus data source using the endpoint: `prom:9090`
1. Enjoy!
