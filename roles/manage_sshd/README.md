# Manage sshd

This role manages the sshd configuration.

 - Disable Root login
 - Disable Password login

## Example Playbook

```yaml
- hosts: all
  gather_facts: false
  become: true
  roles:
    - role: hendrikhuels.cd.manage_sshd
```
