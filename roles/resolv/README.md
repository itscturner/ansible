resolv
======

An ansible role to configure resolv.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Resolv configuration file location:
resolv_conf_file

Name server IP addresses:
resolv_nameservers

Resolv domain:
resolv_domain

Search list for host-name lookup:
resolv_search

Allows addresses returned by gethostbyname to be sorted:
resolv_sortlist

Resolv Options allows certain internal resolver variables to be modified:
resolv_options
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: resolv
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
