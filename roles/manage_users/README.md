# Manage users

This role manages users and dotfiles.

## Configuration

Variable                     | Default                                          | Description
---                          | ---                                              | ---
`manage_users`               | (required)                                       | (`dictionary, list`) List of all users with attributes
`manage_users_primary_group` | `devops`                                         | (`str`) Primary group
`manage_users_groups`        | "systemd-journal,systemd-resolve"                | (`str`) User groups
`manage_users_home_folder`   | `{{ inventory_dir }}/files/project_users/` | (`str`) Directory, where to find the /home mirror
`manage_users_default_admins`| empty                                            | (`list`) List of standard admin users

## Example

Call the role
```yaml
- hosts: all
  gather_facts: false
  become: true
  vars:
    ansible_user: "root"
    project_users_folder: "{{ playbook_dir }}/files/project_users/"
    project_users:
      - { name: "user1", shell: "/bin/bash" }
  roles:
    - role: hendrikhuels.cd.manage_users
```
