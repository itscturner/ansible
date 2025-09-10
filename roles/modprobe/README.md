modprobe
========

An ansible role to configure kernel modules with modprobe.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
List of requirements for modprobe:
modprobe_requirements

List of modprobe modules to install:
modprobe_modules

List of modprobe modules to remove:
modprobe_blacklisted_modules
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: modprobe
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
