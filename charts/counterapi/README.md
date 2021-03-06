# counterapi

![Version: 0.4.0](https://img.shields.io/badge/Version-0.4.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.9.0](https://img.shields.io/badge/AppVersion-v0.9.0-informational?style=flat-square)

A Helm chart for Counter API

**Homepage:** <https://charts.omegion.dev>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| omegion | oomegion@gmail.com |  |

## Source Code

* <https://github.com/counterapi/counterapi>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| deployment.enabled | bool | `false` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/counterapi/counterapi"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths | list | `[]` |  |
| ingress.tls | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| rollout.enabled | bool | `true` |  |
| rollout.envFrom | list | `[]` |  |
| rollout.strategy.canary.steps[0].setWeight | int | `20` |  |
| rollout.strategy.canary.steps[1].pause | object | `{}` |  |
| rollout.strategy.canary.steps[2].setWeight | int | `40` |  |
| rollout.strategy.canary.steps[3].pause.duration | string | `"40s"` |  |
| rollout.strategy.canary.steps[4].setWeight | int | `60` |  |
| rollout.strategy.canary.steps[5].pause.duration | string | `"20s"` |  |
| rollout.strategy.canary.steps[6].setWeight | int | `80` |  |
| rollout.strategy.canary.steps[7].pause.duration | string | `"20s"` |  |
| secret.annotations | object | `{}` |  |
| secret.enabled | bool | `false` |  |
| secret.secrets | list | `[]` |  |
| securityContext | object | `{}` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
