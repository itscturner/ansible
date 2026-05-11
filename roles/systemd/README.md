Systemd
=======

An Ansible role to configure systemd.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Select the target to boot into ("Multiuser", "Graphical" or "Rescue"):
  systemd_target

Options for coredump.conf (Key, Value):
  systemd_coredump

Options for journald.conf. (Key, Value):
  systemd_journald

Options for logind.conf. (Key, Value):
  systemd_logind

Options for system.conf. (Key, Value):
  systemd_system

Options for user.conf. (Key, Value):
  systemd_user
```

Example Playbook
----------------
```
  - hosts: workstations
    roles:
      - role: systemd
        systemd_target: graphical
        systemd_coredump:
          - key: 'Compress'
            value: 'true'        
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
