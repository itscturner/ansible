Systemd
=======

An Ansible role to configure systemd.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```

```

Example Playbook
----------------
```
  - hosts: workstations
    roles:
      - role: systemd
        systemd_target: graphical
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
