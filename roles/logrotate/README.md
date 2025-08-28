logrotate
=========

An ansible role to configure logrotate.

Requirements
------------

None

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`
```
Logrotate package:
logrotate_package

Logrotate configuration directory:
logrotate_directory

How often to rotate logs (Either daily, weekly or monthly):
logrotate_frequency

How many files to keep:
logrotate_keep

Whether to compress rotated logs or not:
logrotate_compress
```

Dependencies
------------

None

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: logrotate
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
