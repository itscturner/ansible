Pip
===

An Ansible role to install and configure Pip.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Required packages to install for pip:
  pip_required_packages

Default Python version:
  pip_python_version

Pip executable path (changes depending on the 'pip_python_version' variable):
  pip_executable

Default timeout value in seconds:
  pip_conf_timeout

Location of the pip log file:
  pip_conf_log_file

Only install pip packages in a virtual environment:
  pip_conf_respect_virtualenv

Download cache location for pip:
  pip_conf_download_cache

Level of verbosity for pip output:
  pip_conf_verbose

Trust a specific host if it doesn't use SSL/TLS:
  pip_conf_trusted_host

Set the primary pip package index:
  pip_conf_index_url

Proxy information for pip:
  pip_conf_proxy

Add an additional pip package index to search if the primary fails:
  pip_conf_extra_index_url

Where pip should look for packages to install:
  pip_conf_find_links

Ignore already installed packages:
  pip_conf_ignore_installed

Always use the '--no-cache-dir' flag for pip installations:
  pip_conf_no_cache_dir
 
Format to display 'pip list' in:
  pip_conf_list_format

Extra configurations to add to the pip configuration file (Section, Option, Value):
  pip_extra_configurations
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: pip
        pip_python_version: '3.9'
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
