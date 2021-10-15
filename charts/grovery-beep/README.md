
# grocery-beep

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0.0](https://img.shields.io/badge/AppVersion-1.0.0-informational?style=flat-square)

> Scan barcodes to add products to your grocery shopping list

**Homepage:** <https://github.com/aolde/grocery-beep>

## Installing the Chart

To install the chart with the release name `my-release`:

```console
$ helm repo add aolde https://aolde.github.io/helm
$ helm install my-release -f values.yaml aolde/grocery-beep
```

Create a `values.yaml` file to customize the chart.

```yaml
# example values.yaml - modify to your needs
podAnnotations:
    prometheus.io/path: "/metrics"
    prometheus.io/port: "80"

```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| annotations | object | `{}` |  |
| config.googleKeepNotesId | string | `""` |  |
| config.mqttHostIp | string | `""` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"Always"` |  |
| image.repository | string | `"ghcr.io/aolde/grocery-beep-be"` |  |
| image.tag | string | `"latest"` | Overrides the image tag whose default is the chart appVersion. |
| imagePullSecrets | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| tolerations | list | `[]` |  |
| volumeMounts | list | `[]` |  |
| volumes | list | `[]` |  |
