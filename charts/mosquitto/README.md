# mosquitto

![Version: 0.7.0](https://img.shields.io/badge/Version-0.7.0-informational?style=flat-square) ![AppVersion: 2.0.4](https://img.shields.io/badge/AppVersion-2.0.4-informational?style=flat-square)

Eclipse Mosquitto - An open source MQTT broker

**Homepage:** <https://mosquitto.org/>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| ishioni | helm@movishell.pl |  |

## Source Code

* <https://github.com/eclipse/mosquitto>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| extraVolumeMounts | list | `[]` |  |
| extraVolumes | list | `[]` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"eclipse-mosquitto"` |  |
| image.tag | string | `"{{ .Chart.AppVersion }}"` |  |
| imagePullSecrets | list | `[]` |  |
| monitoring.podMonitor.enabled | bool | `false` |  |
| monitoring.sidecar.args[0] | string | `"--use-splitted-config"` |  |
| monitoring.sidecar.enabled | bool | `false` |  |
| monitoring.sidecar.envs[0].name | string | `"MQTT_CLIENT_ID"` |  |
| monitoring.sidecar.envs[0].value | string | `"exporter"` |  |
| monitoring.sidecar.envs[1].name | string | `"BROKER_HOST"` |  |
| monitoring.sidecar.envs[1].valueFrom.fieldRef.fieldPath | string | `"status.podIP"` |  |
| monitoring.sidecar.image.pullPolicy | string | `"IfNotPresent"` |  |
| monitoring.sidecar.image.repository | string | `"nolte/mosquitto-exporter"` |  |
| monitoring.sidecar.image.tag | string | `"v0.6.3"` |  |
| monitoring.sidecar.port | int | `9234` |  |
| monitoring.sidecar.resources.limits.cpu | string | `"300m"` |  |
| monitoring.sidecar.resources.limits.memory | string | `"128Mi"` |  |
| monitoring.sidecar.resources.requests.cpu | string | `"100m"` |  |
| monitoring.sidecar.resources.requests.memory | string | `"64Mi"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.annotations | object | `{}` |  |
| persistence.enabled | bool | `false` |  |
| persistence.size | string | `"5Gi"` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.annotations | object | `{}` |  |
| service.port | int | `1883` |  |
| service.type | string | `"ClusterIP"` |  |
| service.websocketPort | int | `9001` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `nil` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
