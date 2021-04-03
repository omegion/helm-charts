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

```shell
vault write ssh-client-signer/config/ca private_key="$(cat ~/.ssh/hetzner)" public_key="$(cat ~/.ssh/hetzner.pub)"

sudo launchctl stop com.openssh.sshd
sudo launchctl start com.openssh.sshd


vault write ssh-client-signer/roles/my-role -<<"EOH"
{
  "allow_user_certificates": true,
  "allowed_users": "*",
  "allowed_extensions": "permit-pty,permit-port-forwarding",
  "default_extensions": [
    {
      "permit-pty": ""
    }
  ],
  "key_type": "ca",
  "default_user": "root",
  "ttl": "30m0s"
}
EOH
```
