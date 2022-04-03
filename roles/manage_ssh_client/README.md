# Manage ssh client config

This role manages ssh config on client.

## Example Playbook

```yaml
- hosts: localhost
  gather_facts: false
  become: true
  roles:
    - role: hendrikhuels.cd.manage_ssh_client
```
