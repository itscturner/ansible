ansible
=======

An ansible role to configure ansible.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
List of ansible packages:
ansible_packages

List of ansible collections:
ansible_collections

Ansible configuration file directory:
ansible_configuration_directory

Ansible configuration file name:
ansible_config_file

Ansible inventory path:
ansible_inventory_path

Ansible roles path:
ansible_roles_path

Ansible library path:
ansible_library_path

Ansible module utils path:
ansible_module_utils_path

Ansible log path:
ansible_log_path

Ansible vault password file location:
ansible_vault_password_file

Ansible system warnings:
ansible_system_warnings

Ansible deprecation warnings:
ansible_deprecation_warnings

Ansible command warnings:
ansible_command_warnings

Ansible cows:
ansible_nocows

List of cows to print:
ansible_cow_selection

Ansible compression level of variables sent to worker processes:
ansible_var_compression_level

Ansible become:
ansible_become

Ansible become method:
ansible_become_method

Ansible become user:
ansible_become_user

Ansible become ask password:
ansible_become_ask_pass

Ansible ssh arguments:
ansible_ssh_args

Ansible pipelining:
ansible_pipelining

```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: ansible
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
