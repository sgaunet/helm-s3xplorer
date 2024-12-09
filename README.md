[![GitHub release](https://img.shields.io/github/release/sgaunet/helm-s3xplorer.svg)](https://github.com/sgaunet/helm-s3xplorer/releases/latest)
![GitHub Downloads](https://img.shields.io/github/downloads/sgaunet/helm-s3xplorer/total)

# helm-s3xplorer

```bash
helm repo add s3xplorer https://sgaunet.github.io/helm-s3xplorer/
helm repo update
helm search repo s3xplorer
```

[Here is the documentation to configure the helm chart.](charts/s3xplorer/README.md)

# Development

This project is using :

* [helm](https://helm.sh/)
* [task for development](https://taskfile.dev/#/)
* [pre-commit](https://pre-commit.com/)

There are hooks executed in the precommit stage. Once the project cloned on your disk, please install pre-commit:

```bash
brew install pre-commit
```

And install the hooks:

```bash
task dev:install-pre-commit
```

If you like to launch manually the pre-commmit hook:

```bash
task dev:pre-commit
```
