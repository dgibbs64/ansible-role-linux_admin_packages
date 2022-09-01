# linux_admin_packages

An [Ansible](https://www.ansible.com) role that:
* installs various useful packages for Linux Administrators on Debian and RedHat based distros.
* adds global basic vimrc from [amix](https://github.com/amix/vimrc).
* adds date stamps to history.
* adds useful bash aliases.

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
