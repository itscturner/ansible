arch
====

An ansible role for arch linux.

Requirements
------------

REQUIREMENTS

Role Variables
--------------

ROLE VARIABLES

Dependencies
------------

DEPENDENCIES

Example Playbook
----------------
```
  - hosts: servers
    roles:
      - role: arch
    when: ansible_os_family == 'Archlinux' or ansible_os_family == 'Arch Linux'
```

License
-------

LICENSE

Author Information
------------------

itscturner
