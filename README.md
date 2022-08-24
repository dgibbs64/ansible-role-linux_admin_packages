# linux_admin_packages

An [Ansible](https://www.ansible.com) role to install various useful packages for Linux Administrators for Debian and RedHat based distros.
As well as add global basic vimrc from [amix](https://github.com/amix/vimrc) and add date stamps to history.

Please see tasks/main.yml for the list of packages installed.

## Requirements

None.

## Role Variables

None.

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
