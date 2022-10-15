# linux_admin_packages

An [Ansible](https://www.ansible.com) role that:

- installs various useful packages for Linux Administrators on Debian and RedHat based distros.
- adds global basic vimrc from [amix](https://github.com/amix/vimrc).
- adds date stamps to history.
- enables systat logging `/var/log/sysstat`.

Packages installed

Please see [vars/main.yml](https://github.com/dgibbs64/ansible-role-linux-admin-packages/blob/main/vars/main.yml) for the list of packages installed.

|GitHub|Quality|Downloads|Version|
|------|-------|---------|-------|
|[![github](https://github.com/dgibbs64/ansible-role-linux_admin_packages/workflows/Ansible%20Molecule/badge.svg)](https://github.com/robertdebock/ansible-role-bootstrap/actions)|[![quality](https://img.shields.io/ansible/quality/59358)](https://galaxy.ansible.com/dgibbs64/linux_admin_packages)|[![downloads](https://img.shields.io/ansible/role/d/59358)](https://galaxy.ansible.com/dgibbs64/linux_admin_packages)|[![Version](https://img.shields.io/github/release/dgibbs64/ansible-role-linux_admin_packages.svg)](https://github.com/dgibbs64/linux_admin_packages/releases/)|

## Requirements

None.

## Role Variables

```yaml
histformat: true
systat_logging_enabled: true
vimrc: true
```

## Dependencies

None.

## Example Playbook

```yaml
---
- name: Linux Admin Packages
  hosts: all
  roles: dgibbs64.linux_admin_packages
```

## License

MIT

## Author Information

- [Daniel Gibbs](https://danielgibbs.co.uk)
