umask
=====

An ansible role to configure umask.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Set default umask:
umask

Which users to set umask:
umask_users
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: umask
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
