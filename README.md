# EVCC Helm chart

This Helm chart deploys EVCC, an open-source electric vehicle charging controller, on a Kubernetes cluster.
The chart derives from https://jitsehijlkema.github.io/evcc-chart/ with few improvements and updates.

## Prerequisites

- Kubernetes 1.16+
- Helm 3.0+

## Installing the Chart

To install the chart with the release name `my-evcc`:

```bash
helm repo add evcc https://evcc.io/helm-charts
helm install my-evcc evcc/evcc
```

## Features

- Configurable EVCC settings via Helm values
- Exposure of OCPP, MQTT, Modbus, and HTTP APIs via services