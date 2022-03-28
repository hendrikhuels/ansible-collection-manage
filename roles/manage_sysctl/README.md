# Manage users

This role manages sysctl settings.

## Configuration

Variable                     | Default                           | Description
---                          | ---                               | ---
`manage_sysctl_path`         | `/etc/sysctl.d/99-devops.conf`    | (`str`) Set sysctl conf path

## Example

Call the role
```yaml
- hosts: all
  gather_facts: false
  become: true
  roles:
    - role: hendrikhuels.cd.manage_sysctl
```
