vscode
======

An ansible role to install and configure VSCode.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
List of VSCode extensions:
vscode_extensions
```

Example Playbook
----------------
```
  - hosts: workstations
    roles:
      - role: vscode
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
