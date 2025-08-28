alternatives
============

An ansible role for alternatives.

Requirements
------------

None

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`
```
List of alternatives packages:
alternatives_packages

List of alternatives:
alternatives_list
```

Dependencies
------------

None

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: alternatives
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
