# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.3.0]
### Added
 - Added role manage_hosts
 - Added role manage_ssh_bastion

### Change
 - Change default vaule of manage_users_home_folder from null to `{{ inventory_dir }}/../../files/project_users/`

## [0.2.0]
### Added
 - Added role manage_tools
 - Added role manage_sysctl

## [0.1.0]
### Added
 - Added role manage_users