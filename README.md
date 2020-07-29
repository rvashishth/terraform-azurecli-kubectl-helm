# terraform-azurecli-kubectl-helm
Small Alpine based Docker image with Terraform, azure-cli, kubectl and Helm.

# Docker Hub
[ventx/terraform-azurecli-kubectl-helm](https://hub.docker.com/r/ventx/terraform-azurecli-kubectl-helm)

# Docker image
* OS: Alpine
* Version: 3.11

# Installed packages (apk)
* [python3](https://pkgs.alpinelinux.org/package/v3.11/main/x86_64/python3)
* [curl](https://pkgs.alpinelinux.org/package/v3.11/main/x86_64/curl)
* [git](https://pkgs.alpinelinux.org/package/v3.11/main/x86_64/git)
* [jq](https://pkgs.alpinelinux.org/package/v3.11/main/x86_64/jq)
* [gettext](https://pkgs.alpinelinux.org/package/v3.11/main/x86_64/gettext)

# Installed packages (pip)
* [azure-cli](https://pypi.org/project/azure-cli) `2.7.0`

# Installed packages (go binaries)
* [terraform](https://www.terraform.io/downloads.html) `0.12.29`
* [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/) `v1.16.10`
* [helm](https://github.com/helm/helm/releases) `v3.0.3`
