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

1. Head to `localhost:3000` (default username: `admin`, pw: `admin`)
1. Add the prometheus data source using the URL: `http://prom:9090`
1. Click `Save and Test`.
1. Enjoy!
