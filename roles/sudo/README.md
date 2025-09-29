sudo
====

An ansible role to install and configure sudo.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
List of sudo packages:
sudo_packages

Path of the sudoers configuration file:
sudo_sudoers_file

Path of the sudoers.d directory:
sudo_sudoersd_directory

Sudoers host aliases:
sudo_sudoers_host_aliases

Suoders user aliases:
sudo_sudoers_user_aliases

Sudoers command aliases:
sudo_sudoers_command_aliases

Sudoers defaults.
sudo_sudoers_defaults

Sudoers ENV keep list:
sudo_sudoers_env_keep

Sudoers secure path:
sudo_sudoers_secure_path

Sudoers user specifications:
sudo_sudoers_user_specification

Sudoers group specifications:
sudo_sudoers_group_specification
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: sudo
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
