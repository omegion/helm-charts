# vault-unseal-cronjob

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.1.0](https://img.shields.io/badge/AppVersion-0.1.0-informational?style=flat-square)

A chart for unseal Vault cron job

**Homepage:** <https://github.com/omegion>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| omegion | oomegion@gmail.com |  |

## Source Code

* <https://github.com/omegion>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| image.name | string | `"ghcr.io/omegion/vault-unseal"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.tag | string | `"v0.1.0"` |  |
| restartPolicy | string | `"OnFailure"` |  |
| schedule | string | `"\"*/30 * * * *\""` |  |
| successfulJobsHistoryLimit | int | `3` |  |
| vault.address | string | `""` |  |
| vault.shards | list | `[]` |  |

