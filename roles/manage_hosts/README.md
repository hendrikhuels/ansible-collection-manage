# Manage users

This role manages hosts file.

## Example

Call the role
```yaml
- hosts: all
  gather_facts: false
  become: true
  roles:
    - role: hendrikhuels.cd.manage_hosts
```
