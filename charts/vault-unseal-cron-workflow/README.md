# vault-unseal-cron-workflow

![Version: 0.6.0](https://img.shields.io/badge/Version-0.6.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.6.0](https://img.shields.io/badge/AppVersion-0.6.0-informational?style=flat-square)

A chart for unseal Vault cron workflow in Argo Workflows

**Homepage:** <https://charts.omegion.dev>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| omegion | oomegion@gmail.com |  |

## Source Code

* <https://github.com/omegion/vault-unseal>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| image.name | string | `"ghcr.io/omegion/vault-unseal"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.tag | string | `"v0.3.0"` |  |
| schedule | string | `"\"*/30 * * * *\""` |  |
| serviceAccountName | string | `"argo-workflow"` |  |
| vault.address | string | `""` |  |
| vault.shards | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)