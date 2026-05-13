Pip
===

An Ansible role to install and configure Pip.

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`

| Variable           | Required | Default                                | Choices | Comments                                                                      |
|--------------------|----------|----------------------------------------|---------|-------------------------------------------------------------------------------|
| pip_python_version | yes      |                                        |         | Python version.                                                               |
| pip_executable     | no       | "/usr/bin/pip{{ pip_python_version }}" |         | Pip executable path (changes depending on the 'pip_python_version' variable). |
| pip_configurations | no       |                                        |         | Configurations to add to pip.conf (Section, Option, Value).                   |

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
