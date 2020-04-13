# IBM Security Helm Charts Repository

## Overview

The IBM-Security *helm-charts* repository contains Helm charts which can be used to deploy IBM-Security images into a Kubernetes environment. Further information on Helm charts can be found in the official documentation: [https://helm.sh/docs/topics/charts/](https://helm.sh/docs/topics/charts/).

The `stable` directory contains Helm chart source provided by IBM, while the `repo/stable` directory contains the packaged Helm chart binaries. 

To add the stable repo to the local repository list run the following command :

```shell
helm repo add stable https://raw.githubusercontent.com/IBM-Security/helm-charts/master/repo/stable
```