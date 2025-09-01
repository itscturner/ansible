password
========

An ansible role to configure password policies.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Password quality file location:
password_complexity_file

Login definitions file location:
password_logindefs_file
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: password
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
