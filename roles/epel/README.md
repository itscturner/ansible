epel
====

An ansible role to configure epel.

Requirements
------------

None.

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`
```
EPEL repo file path:
epel_repofile

EPEL repo GPG key:
epel_repo_gpg_key

EPEL repo URL:
epel_repo_url
```

Dependencies
------------

None.

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: epel
    when: ansible_os_family == 'RedHat'
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
