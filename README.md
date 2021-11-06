Ansible role: solana
=========

This role helps you to install minikube on your linux machine.


|Travis|GitHubActions|Quality|Downloads|Version|
|------|-------------|-------|---------|-------|
|[![travis](https://travis-ci.com/amine7777/ansible-role-solana.svg?branch=master)](https://travis-ci.com/amine7777/ansible-role-solana)|[![github](https://github.com/amine7777/ansible-role-solana/workflows/CI/badge.svg)](https://github.com/amine7777/ansible-role-solana/actions)|[![quality](https://img.shields.io/ansible/quality/49942)](https://galaxy.ansible.com/amine7777/solana)|[![downloads](https://img.shields.io/ansible/role/d/50348)](https://galaxy.ansible.com/amine7777/solana)|[![Version](https://img.shields.io/github/release/amine7777/ansible-role-solana.svg)](https://github.com/amine7777/ansible-role-solana/releases/)|

![](solana.png)

Requirements
------------
- Linux machine
- Ansible 2.10

Role Variables
--------------
These variables helps to manage solana installation.

You can specify your solana version in this variable.
```yaml
solana_version: 1.6.4
solana_arch: amd64
solana_directory_path: /usr/local/bin
```
This is the url where solana will be downloaded.
```yaml
solana_download_url: 'https://releases.hashicorp.com/solana/{{ solana_version }}/solana_{{ solana_version }}_linux_{{ solana_arch }}.zip'
```
This is the path where solana binary will be stored.
```yaml
solana_directory_path: /usr/local/bin
```

Example Playbook
----------------

```yaml
- hosts: all
  roles:
     - amine7777.solana
```


Author Information
------------------

- [Amine Kahlaoui](https://github.com/amine7777), DevOps engineer.
