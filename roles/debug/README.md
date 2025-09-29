debug
=====

An ansible role for debugging.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Show all variables:
debug_all_variables

Show specific variable:
debug_variable
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: debug
        debug_variable: ansible_distribution_major_version
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
