ansible-container-engine
========================

Ansible playbook for Docker and Kubernetes

Supported distributions:

- Fedora
- CentOS
- Ubuntu

Setup
-----

```sh
$ git clone https://github.com/dceoy/ansible-container-engine.git
$ cd ansible-container-engine
$ cp example_hosts hosts
$ vim hosts               # => edit
$ cp example_vars.yml group_vars/all.yml
$ vim group_vars/all.yml  # => edit
```

Usage
-----

Provision servers with Docker and Kubernetes

```sh
$ ansible-playbook -i hosts provision.yml
```
