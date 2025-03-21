# s3xplorer

![Version: 0.4.1](https://img.shields.io/badge/Version-0.4.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.4.1](https://img.shields.io/badge/AppVersion-0.4.1-informational?style=flat-square)

A Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| additionalAnnotations | object | `{}` | additional annotations |
| additionalEnvFrom | list | `[]` | additional configmap or secret.  |
| additionalLabels | object | `{}` | additional deployment labels (will be merged with the default labels) |
| affinity | object | `{}` |  |
| configuration.accesskey | string | `""` | access key for the aws credentials |
| configuration.apikey | string | `""` | api key for the aws credentials |
| configuration.bucket | string | `"my-bucket"` | bucket name |
| configuration.loglevel | string | `"info"` | debug or info or warn or error |
| configuration.prefix | string | `""` | set the prefix to restrict the access to a specific folder |
| configuration.s3endpoint | string | `""` | s3 endpoint |
| configuration.s3region | string | `"eu-west-3"` | region of the s3 bucket |
| configuration.ssoawsprofile | string | `""` | in case of helm deployment, ssoawsprofile should be left empty |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"sgaunet/s3xplorer"` | image repository |
| image.tag | string | `""` | Overrides the image tag whose default is the chart appVersion. |
| imagePullSecrets | list | `[]` | image pull secrets |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` | number of replicas |
| resources.limits.cpu | string | `"300m"` |  |
| resources.limits.memory | string | `"128Mi"` |  |
| resources.requests.cpu | string | `"100m"` |  |
| resources.requests.memory | string | `"64Mi"` |  |
| securityContext | object | `{}` |  |
| service.port | int | `8081` |  |
| service.type | string | `"ClusterIP"` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
