ulimit
======

An Ansible role to configure ulimit.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Default domain for limits configuration file:
  ulimit_domain

Default limit type for limits configuration file:
  ulimit_limit_type

The filepath of the limits configuration file:
  ulimit_file

Backup limits.conf when changes occur:
  ulimit_backup

Configurations for ulimit (Domain - defaults to 'ulimit_domain', Type - defaults to 'ulimit_limit_type', Limit Item, Value):
  ulimit_configurations
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: ulimit
        ulimit_configurations:
          - domain: root
            type: hard
            limit_item: nproc
            value: 2048
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
