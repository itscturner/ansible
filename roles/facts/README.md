facts
=====

An ansible role for creating custom facts.

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`
```
List of custom facts:
facts
```

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

Apache-2.0

Author Information
------------------

itscturner
