# gcppromd

![Version: v1.0.3](https://img.shields.io/badge/Version-v1.0.3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.4.0](https://img.shields.io/badge/AppVersion-v0.4.0-informational?style=flat-square)

A Helm chart for gcppromd

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| steinbrueckri | richard.steinbrueck@gmail.com |  |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| image.repository | string | `"messagebird/gcppromd"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| nameOverride | string | `""` |  |
| fullnameOverride | string | `""` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.name | string | `""` |  |
| gcppromd.frequency | int | `400` |  |
| gcppromd.outputFileName | string | `"targets.json"` |  |
| gcppromd.projects | list | `[]` |  |
| gcppromd.projectsAutoDiscovery | bool | `true` |  |
| gcppromd.projectsExcludes | string | `""` |  |
| gcppromd.worker | string | `"30"` |  |
| serviceAccountKey | string | `""` |  |
| existingSecret | string | `""` |  |
| existingSecretKey | string | `""` |  |
| podSecurityContext.fsGroup | int | `1000` |  |
| securityContext.runAsUser | int | `1000` |  |
| resources | object | `{}` |  |
| nodeSelector | object | `{}` |  |
| tolerations | list | `[]` |  |
| affinity | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| serviceAnnotations | object | `{}` |  |
| serviceLabels | object | `{}` |  |
| serviceAccountLabels | object | `{}` |  |
| persistentVolumeLabels | object | `{}` |  |
| persistentVolume.enabled | bool | `true` |  |
| persistentVolume.accessModes[0] | string | `"ReadWriteOnce"` |  |
| persistentVolume.annotations | object | `{}` |  |
| persistentVolume.existingClaim | string | `""` |  |
| persistentVolume.mountPath | string | `"/data"` |  |
| persistentVolume.size | string | `"2Gi"` |  |
| networkPolicy | object | `{}` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)