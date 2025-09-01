ulimit
======

An ansible role to configure ulimit.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Configuration file location:
ulimit_conf

Create a backup of limits.conf on changes:
ulimit_backup

Default domain:
ulimit_domain

Default limit type:
ulimit_limit_type

Ulimit configurations:
ulimit_configurations
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: ulimit
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
