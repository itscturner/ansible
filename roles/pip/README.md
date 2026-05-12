Pip
===

An Ansible role to install and configure Pip.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Required packages to install for pip:
  pip_required_packages

Python version:
  pip_python_version

Pip executable path (changes depending on the 'pip_python_version' variable):
  pip_executable

Configurations to add to pip.conf (Section, Option, Value):
  pip_configurations
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: pip
        pip_python_version: '3.12'
        pip_configurations:
          - section: global
            option: index-url
            value: 'https://pypi.org/simple'
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
