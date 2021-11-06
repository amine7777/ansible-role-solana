Ansible role: solana
=========

This role helps you to install solana on your linux machine.


|Travis|GitHubActions|Quality|Downloads|Version|
|------|-------------|-------|---------|-------|
|[![travis](https://travis-ci.com/amine7777/ansible-role-solana.svg?branch=master)](https://travis-ci.com/amine7777/ansible-role-solana)|[![github](https://github.com/amine7777/ansible-role-solana/workflows/CI/badge.svg)](https://github.com/amine7777/ansible-role-solana/actions)|[![quality](https://img.shields.io/ansible/quality/49942)](https://galaxy.ansible.com/amine7777/solana)|[![downloads](https://img.shields.io/ansible/role/d/50348)](https://galaxy.ansible.com/amine7777/solana)|[![Version](https://img.shields.io/github/release/amine7777/ansible-role-solana.svg)](https://github.com/amine7777/ansible-role-solana/releases/)|

![](solana.png)

Requirements
------------
- Linux machine
- Ansible 2.11

Role Variables
--------------
These variables helps to manage solana installation.

You can specify your solana version in this variable.
```yaml
solana_version: v1.8.2
```
This is the url where solana will be downloaded.
```yaml
solana_install_url: "https://release.solana.com/{{ solana_version }}/install"
```
This is the path where solana binary will be stored.
```yaml
solana_bin_path: ~/.local/share/solana/install/active_release/bin
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
