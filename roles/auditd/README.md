auditd
======

An ansible role to configure auditd.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Auditd service name:
auditd_service

Auditd configuration directory:
auditd_config_directory

Auditd configuration file:
auditd_config_file
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: auditd
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
