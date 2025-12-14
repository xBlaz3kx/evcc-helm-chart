# EVCC Helm chart

This Helm chart deploys [EVCC](https://evcc.io/), an open-source electric vehicle charging controller, on a Kubernetes
cluster.
The chart derives from https://jitsehijlkema.github.io/evcc-chart/ with few improvements and updates.

## Prerequisites

- Kubernetes 1.16+
- Helm 3.0+
- EVCC version 0.211.2 or higher

Using EVCC versions prior to 0.211.2 are incompatible with this chart due issues in database DSN parsing.

## Installing the Chart

To install the chart with the release name `my-evcc`:

```bash
helm repo add evcc https://helm.blazdular.cc/charts
helm install my-evcc evcc/evcc
```

## Features

- Configurable EVCC settings via Helm values
- Exposure of OCPP, MQTT, Modbus, and HTTP APIs via services
- Configurable SQLite database remote backups