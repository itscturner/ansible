epel
====

An ansible role to configure epel.

Requirements
------------

REQUIREMENTS

Role Variables
--------------

ROLE VARIABLES

Dependencies
------------

DEPENDENCIES

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: epel
    when: ansible_os_family == 'RedHat'
```

License
-------

LICENSE

Author Information
------------------

itscturner
