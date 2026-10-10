# Ansible Restic

This role installs the [restic](https://github.com/restic/restic) backup binary and its required runtime dependencies on Debian-based systems.

## Installation

Install from Ansible Galaxy:

```bash
ansible-galaxy role install sebastian13.restic -p roles
```

Or clone it locally:

```bash
git clone https://github.com/sebastian13/ansible-restic.git roles/restic
```

## Example Playbook

```yaml
---
- name: Install restic
  hosts: restic_servers
  become: true

  roles:
    - role: sebastian13.restic
```

## Requirements

- A supported Debian-based host
- Root privileges via `become: true`

## Resources

- [restic/restic](https://github.com/restic/restic)
- [restic.net](https://restic.net/)
- This role is based on the original work by [donat-b/ansible-restic](https://github.com/donat-b/ansible-restic).
