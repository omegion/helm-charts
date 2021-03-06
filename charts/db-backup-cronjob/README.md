# db-backup-cronjob

![Version: 0.11.0](https://img.shields.io/badge/Version-0.11.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.11.0](https://img.shields.io/badge/AppVersion-0.11.0-informational?style=flat-square)

A chart for creating database backup and upload t o S3

**Homepage:** <https://charts.omegion.dev>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| omegion | oomegion@gmail.com |  |

## Source Code

* <https://github.com/omegion/db-backup>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| container.args | list | `[]` |  |
| container.command | list | `[]` |  |
| image.name | string | `"ghcr.io/omegion/db-backup"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.tag | string | `"v0.9.0"` |  |
| podAnnotations | object | `{}` |  |
| restartPolicy | string | `"OnFailure"` |  |
| schedule | string | `"\"*/30 * * * *\""` |  |
| serviceAccount.name | string | `""` |  |
| successfulJobsHistoryLimit | int | `3` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
