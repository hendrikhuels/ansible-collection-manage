# Manage users

This role manages installed tools.

## Configuration

Variable                     | Default       | Description
---                          | ---           | ---
`manage_tools_packages`      | `['podman', 'bash-completion']`  | (`list`) Installed software
`manage_tools_epel_release`  | `false`        | (`bool`) Install epel-release


## Example

Call the role
```yaml
- hosts: all
  gather_facts: false
  become: true
  vars:
    manage_tools_packages: ['podman', 'skopeo', 'net-tools']
    manage_tools_epel_release: true
  roles:
    - role: hendrikhuels.cd.manage_tools
```
