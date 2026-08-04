# linux_admin_packages

An [Ansible](https://www.ansible.com) role that installs useful packages for Linux Administrators

<!-- markdownlint-disable MD013 -->
<p align="center">
<a href="https://github.com/dgibbs64/ansible-role-linux_admin_packages/actions/workflows/action-molecule.yml"><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/dgibbs64/ansible-role-linux_admin_packages/action-molecule.yml?label=molecule&logo=ansible&style=flat-square"></a> <a href="https://galaxy.ansible.com/dgibbs64/linux_admin_packages"><img alt="GitHub tag (latest by date)" src="https://img.shields.io/github/v/tag/dgibbs64/ansible-role-linux_admin_packages?color=EE0000&label=release&logo=ansible&style=flat-square"></a>
<a href="/LICENSE.md"><img src="https://img.shields.io/github/license/dgibbs64/ansible-role-linux_admin_packages?style=flat-square" alt="MIT License"></a>
</p>
<!-- markdownlint-enable MD013 -->

## About

This role:

- installs various useful packages for Linux Administrators on Debian, RedHat, and openSUSE based distros.
- adds global basic vimrc from [amix](https://github.com/amix/vimrc).
- adds date stamps to history.
- enables systat logging `/var/log/sysstat`.
- installs neovim, removes other vi/vim packages and can disable mouse support for current and root user.
- installs [fastfetch](https://github.com/fastfetch-cli/fastfetch) on supported distros (replaces the archived neofetch).

Please see [vars/main.yml](https://github.com/dgibbs64/ansible-role-linux_admin_packages/blob/main/vars/main.yml) for the list of packages installed.

## Requirements

None.

## Role Variables

```yaml
---
history_time_format: true
systat_logging_enabled: true
vimrc: true
epel_repofile_path: "/etc/yum.repos.d/epel.repo"
disable_neovim_mouse_support: false
```

## Dependencies

None.

## Example Playbook

```yaml
---
- name: Linux Admin Packages
  hosts: all
  roles:
    - role: "dgibbs64.linux_admin_packages"
```

## License

MIT

## Author Information

- [Daniel Gibbs](https://danielgibbs.co.uk)
