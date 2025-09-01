selinux
=======

An ansible role to install and configure selinux.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
List of SELinux packages:
selinux_packages

SELinux state: enforcing, permissive, or disabled:
selinux_state

SELinux policy:
selinux_policy

You can enable (or disable) booleans by specifying them in this list:
selinux_booleans

Should the machine be rebooted after changes?:
selinux_reboot
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: selinux
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
