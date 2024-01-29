# Ansible Restic

This role deploys the [restic backup](https://github.com/restic/restic) binary after installing all requirements.

## Example Playbook

```yaml
---

- name: Restic
  hosts: restic_servers
  become: true

  roles:
    - sebastian13.restic
```

## Ressources

- [restic/restic](https://github.com/restic/restic)
- [restic.net](https://restic.net/)
- This role is a fork of [donat-b/ansible-restic](https://github.com/donat-b/ansible-restic).
