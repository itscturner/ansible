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
Logrotate package name:
logrotate_package

Logrotate service name.
logrotate_service

Logrotate configuration directory:
logrotate_directory

How often to rotate logs (Either daily, weekly or monthly):
logrotate_frequency

How many files to keep:
logrotate_keep

Whether to compress rotated logs or not:
logrotate_compress

Whether to use date extension on log file names or not:
logrotate_dateext
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
