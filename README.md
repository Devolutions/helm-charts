# Devolutions Kubernetes Helm Charts

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

Official Helm chart repository for Devolutions.

## Usage

[Helm](https://helm.sh) must be installed to use these charts.
Please refer to the Helm [documentation](https://helm.sh/docs/) to get started.

Once Helm is set up properly, add the repository:

```console
helm repo add devolutions https://devolutions.github.io/helm-charts
helm repo update
```

You can then list the available charts:

```console
helm search repo devolutions
```

Example installation:

```console
helm install devolutions-server devolutions/devolutions-server
```

## Available charts

| Chart | Description |
| --- | --- |
| `devolutions-server` | [Devolutions Server](https://devolutions.net/server/) Helm chart |
| `dvls-kubernetes-operator` | Devolutions Server Kubernetes Operator |

## Contributing

We'd love to have you contribute! Please refer to our [contribution guidelines](./CONTRIBUTING.md) for details.

## License

[Apache 2.0 License](./LICENSE).
