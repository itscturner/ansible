check-variables
===============

An ansible role to check variables.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Variable from defaults:
check-variables-default-variable

Variable from vars:
check-variables-vars-variable
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: check-variables
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
