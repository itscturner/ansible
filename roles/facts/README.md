Facts
=====

An ansible role to create custom facts.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Custom facts to create in key/value format:
  facts
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: facts
        vars:
          facts:
            - key: server_location
              value: Denver
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
