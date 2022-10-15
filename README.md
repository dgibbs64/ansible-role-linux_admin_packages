# linux_admin_packages

An [Ansible](https://www.ansible.com) role that:

- installs various useful packages for Linux Administrators on Debian and RedHat based distros.
- adds global basic vimrc from [amix](https://github.com/amix/vimrc).
- adds date stamps to history.
- enables systat logging `/var/log/sysstat`.

Packages installed

Please see [vars/main.yml](https://github.com/dgibbs64/ansible-role-linux-admin-packages/blob/main/vars/main.yml) for the list of packages installed.

## Requirements

None.

## Role Variables

```
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
