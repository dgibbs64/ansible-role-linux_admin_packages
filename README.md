# linux_admin_packages

An [Ansible](https://www.ansible.com) role that:

- installs various useful packages for Linux Administrators on Debian and RedHat based distros.
- adds global basic vimrc from [amix](https://github.com/amix/vimrc).
- adds date stamps to history.
- enables systat logging `/var/log/sysstat`.

Packages installed:

Please see [vars/main.yml](https://github.com/dgibbs64/ansible-role-linux_admin_packages/blob/main/vars/main.yml) for the list of packages installed.

<p align="center">
<a href="https://app.codacy.com/gh/dgibbs64/ansible-role-linux_admin_packages"><img src="https://img.shields.io/codacy/grade/1a892d499efd4dabb73beffa8d64ed01?logo=codacy&style=flat-square" alt="Codacy grade"></a>
<a href="https://github.com/dgibbs64/ansible-role-linux_admin_packages/actions/workflows/molecule.yml"><img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/dgibbs64/ansible-role-linux_admin_packages/Ansible%20Molecule?label=molecule&logo=ansible&style=flat-square"></a>
<a href="https://galaxy.ansible.com/dgibbs64/linux_admin_packages"><img alt="Ansible Quality Score" src="https://img.shields.io/ansible/quality/59356?logo=ansible&style=flat-square"></a>
<a href="https://galaxy.ansible.com/dgibbs64/linux_admin_packages"><img alt="Ansible Role" src="https://img.shields.io/ansible/role/d/59356?color=EE0000&logo=ansible&style=flat-square"></a>
<a href="https://galaxy.ansible.com/dgibbs64/linux_admin_packages"><img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/dgibbs64/ansible-role-linux_admin_packages?logo=ansible&logoColor=github&style=flat-square"></a>
<a href="/LICENSE.md"><img src="https://img.shields.io/github/license/dgibbs64/ansible-role-linux_admin_packages?style=flat-square" alt="MIT License"></a>
</p>

## Requirements

None.

## Role Variables

```yaml
---
history_time_format: true
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
