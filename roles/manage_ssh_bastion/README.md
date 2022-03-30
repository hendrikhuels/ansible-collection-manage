# Manage ssh config

This role manages ssh config on bastion.

## Example Playbook

```yaml
- hosts: localhost
  gather_facts: false
  become: true
  roles:
    - role: hendrikhuels.cd.manage_ssh_bastion
```
