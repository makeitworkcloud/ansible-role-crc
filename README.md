# ansible-role-crc

Ansible role deploying OpenShift Local (CRC) with custom DNS, TLS certificates, OpenShift GitOps (ArgoCD), and KSOPS for encrypted secret management. Deploys as a regular user with sudo access on a RHEL-based system.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [crc_argocd_age_keys](#crc_argocd_age_keys)
  - [crc_argocd_app_branch](#crc_argocd_app_branch)
  - [crc_argocd_app_path](#crc_argocd_app_path)
  - [crc_argocd_app_repo](#crc_argocd_app_repo)
  - [crc_cpus](#crc_cpus)
  - [crc_disk_size](#crc_disk_size)
  - [crc_external_domain](#crc_external_domain)
  - [crc_kubeadmin_password](#crc_kubeadmin_password)
  - [crc_memory](#crc_memory)
  - [crc_pull_secret](#crc_pull_secret)
  - [crc_version](#crc_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.1`

## Default Variables

### crc_argocd_age_keys

#### Default value

```YAML
crc_argocd_age_keys: ''
```

### crc_argocd_app_branch

#### Default value

```YAML
crc_argocd_app_branch: main
```

### crc_argocd_app_path

#### Default value

```YAML
crc_argocd_app_path: bootstrap
```

### crc_argocd_app_repo

#### Default value

```YAML
crc_argocd_app_repo: https://github.com/makeitworkcloud/kustomize-cluster.git
```

### crc_cpus

#### Default value

```YAML
crc_cpus: 10
```

### crc_disk_size

#### Default value

```YAML
crc_disk_size: 500
```

### crc_external_domain

#### Default value

```YAML
crc_external_domain: makeitwork.cloud
```

### crc_kubeadmin_password

#### Default value

```YAML
crc_kubeadmin_password: crc
```

### crc_memory

#### Default value

```YAML
crc_memory: 57344
```

### crc_pull_secret

#### Default value

```YAML
crc_pull_secret: ''
```

### crc_version

#### Default value

```YAML
crc_version: latest
```

## Discovered Tags

**_certs_**

## Dependencies

None.

## License

GPL-3.0-or-later

## Author

xnoto
