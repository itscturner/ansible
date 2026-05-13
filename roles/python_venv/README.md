Python Virtual Environment
==========================

An Ansible role to configure a Python virtual environment.

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`

| Variable                                | Required | Default | Choices | Comments                                                                                                                 |
|-----------------------------------------|----------|---------|---------|--------------------------------------------------------------------------------------------------------------------------|
| python_venv_version                     | yes      |         |         | Python version.                                                                                                          |
| python_venv_base_directory              | yes      | /opt    |         | Base directory for the Python virtual environment.                                                                       |
| python_venv_env_name                    | yes      |         |         | Name of the Python virtual environment.                                                                                  |
| python_venv_user                        | yes      |         |         | User for the Python virtual environment.                                                                                 |
| python_venv_group                       | yes      |         |         | Group for the Python virtual environment.                                                                                |
| python_venv_requirements_file_package   | no       |         |         | List of packages to be added to the requirements.txt file in the Python virtual environment. (Name, Version - optional). |

Example Playbook
----------------

```
  - hosts: all
    roles:
      - role: python_venv
        python_venv_version: '3.12'
        python_venv_env_name: venv
        python_venv_user: cturner
        python_venv_group: cturner

```

License
-------

Apache-2.0

Author Information
------------------

itscturner
