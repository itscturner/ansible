patching
========

An ansible role to patch packages.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
List of packages to update:
patching_package_list

Message to be displayed when patching is complete, and system is rebooting:
patching_reboot_message
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: patching
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
