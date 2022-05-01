# Webapp Helm Chart

A Helm chart for deploying Kubernetes resources for Webapp

## Values

| Key | Type | Default |
|-----|------|---------|
| `application.name` | string | `""` |
| `appversion` | string | `""` |
| `image.pullPolicy` | string | `"Always"` |
| `image.repository` | string | `""` |
| `replicaCount` | int | `1` |
