# ansible-role-crc

Ansible role deploying OpenShift Local (CRC) with custom DNS, TLS certificates, OpenShift GitOps (ArgoCD), and KSOPS for encrypted secret management. Deploys as a regular user with sudo access on a RHEL-based system.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [crc_cpus](#crc_cpus)
  - [crc_disk_size](#crc_disk_size)
  - [crc_external_domain](#crc_external_domain)
  - [crc_gitops_age_keys](#crc_gitops_age_keys)
  - [crc_gitops_bootstrap_path](#crc_gitops_bootstrap_path)
  - [crc_gitops_repo_branch](#crc_gitops_repo_branch)
  - [crc_gitops_repo_url](#crc_gitops_repo_url)
  - [crc_gitops_workloads_path](#crc_gitops_workloads_path)
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

### crc_gitops_age_keys

#### Default value

```YAML
crc_gitops_age_keys: ''
```

### crc_gitops_bootstrap_path

#### Default value

```YAML
crc_gitops_bootstrap_path: bootstrap
```

### crc_gitops_repo_branch

#### Default value

```YAML
crc_gitops_repo_branch: main
```

### crc_gitops_repo_url

#### Default value

```YAML
crc_gitops_repo_url: ''
```

### crc_gitops_workloads_path

#### Default value

```YAML
crc_gitops_workloads_path: workloads
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
