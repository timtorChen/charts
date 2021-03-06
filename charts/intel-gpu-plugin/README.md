# intel-gpu-plugin

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![AppVersion: 0.18.1](https://img.shields.io/badge/AppVersion-0.18.1-informational?style=flat-square)

The Intel GPU plugin facilitates offloading the processing of computation intensive workloads to GPU hardware

**Homepage:** <https://github.com/k8s-at-home/charts/tree/master/charts/intel-gpu-plugin>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| billimek | jeff@billimek.com |  |

## Source Code

* <https://github.com/intel/intel-device-plugins-for-kubernetes/blob/master/cmd/gpu_plugin>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"intel/intel-gpu-plugin"` |  |
| image.tag | string | `"0.18.1"` |  |
| imagePullSecrets | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
