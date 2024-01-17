# kopia

Install and configure [kopia](https://github.com/kopia/kopia) - a cross-platform
backup tool for Windows, macOS & Linux with fast, incremental backups,
client-side end-to-end encryption, compression and data deduplication.

|GitHub|Downloads|Version|
|------|---------|-------|
|[![github](https://github.com/balling-dev/ansible-role-kopia/workflows/Continuous%20Integration/badge.svg)](https://github.com/balling-dev/ansible-role-kopia/actions)|[![downloads](https://img.shields.io/ansible/role/d/balling-dev/kopia)](https://galaxy.ansible.com/ui/standalone/roles/balling-dev/kopia)|[![Version](https://img.shields.io/github/release/balling-dev/ansible-role-kopia.svg)](https://github.com/balling-dev/ansible-role-kopia/releases/)|

## Example Playbook

This example is taken from
[`molecule/default/converge.yml`](
https://github.com/balling-dev/ansible-role-kopia/blob/main/molecule/default/converge.yml)
and is tested on each push, pull request and release.

```yaml
---
- name: "Converge"
  hosts: "all"
  become: true
  gather_facts: true

  roles:
    - role: "balling-dev.kopia"
```

## Role Variables

The default values for the variables are set in
[`defaults/main.yml`](https://github.com/balling-dev/ansible-role-kopia/blob/main/defaults/main.yml):

```yaml
---
# Defaults file for kopia

# Version of kopia to install. Use "latest" to install latest version.
kopia_version: "latest"
```
