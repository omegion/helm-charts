# Omegion Helm Charts

[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/omegion/helm-charts)](https://github.com/omegion/helm-charts/releases/latest)
[![License](https://img.shields.io/github/license/omegion/helm-charts)](https://opensource.org/licenses/AGPL-3.0)

Automated dependency updates. Multi-platform and multi-language.

This repository hosts Omegion's [Helm](https://helm.sh) charts. Chart documentation is automatically generated using [helm-docs](https://github.com/norwoodj/helm-docs)

## Add Helm repository

```shell
helm repo add omegion https://charts.omegion.dev
helm repo update
```

## Install chart

Using config from a file:

```shell
helm install --generate-name omegion/vault-unseal-cronjob --values values.yaml
```
