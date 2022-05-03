# Webapp Helm Chart

A Helm chart for deploying following Kubernetes resources for Webapp:

## Kubernetes resources
| ResourceType | Description|
|-----|------|
| `Deployment` | This create pods for running the container image with `httpd` server
| `Service` | This is `LoadBalancer` type of service, it will route public traffic to the deployment over HTTP - Port 80
| `ConfigMap` | This stores the `index.html` that will be displayed by the `httpd` server

## Values for Helm chart

| Key | Type | Default |
|-----|------|---------|
| `application.name` | string | `""` |
| `appversion` | string | `""` |
| `image.pullPolicy` | string | `"Always"` |
| `image.repository` | string | `""` |
| `replicaCount` | int | `1` |
