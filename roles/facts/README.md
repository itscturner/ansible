facts
=====

An ansible role for creating custom facts.

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
  - hosts: servers
    roles:
      - role: facts
        facts:
          - key: machine_type
            value: server
    
```

License
-------

LICENSE

Author Information
------------------

itscturner
