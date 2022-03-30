# Manage hosts

This role manages hosts file, based on the inventory.

## Example Playbook

```yaml
- hosts: all
  gather_facts: false
  become: true
  roles:
    - role: hendrikhuels.cd.manage_hosts
```
