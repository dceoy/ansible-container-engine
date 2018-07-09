ansible-container-engine
========================

Ansible playbook for Docker, NVIDIA Docker and Kubernetes

Supported distributions:

- Fedora (> 28)
- CentOS (> 7)
- RHEL (> 7)
- Ubuntu (> 18.04)

Setup
-----

```sh
$ git clone https://github.com/dceoy/ansible-container-engine.git
$ cd ansible-container-engine
$ cp example_hosts hosts
$ cp example_vars.yml group_vars/all.yml
$ vim hosts                 # => edit
$ vim group_vars/all.yml    # => edit
```

Usage
-----

Provision servers with Docker and Kubernetes

```sh
$ ansible-playbook -i hosts provision.yml
```

Disabling SELinux is required in CentOS, RHEL, or Fedora (until SELinux support is improved in the kubelet).
