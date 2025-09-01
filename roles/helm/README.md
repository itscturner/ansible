helm
====

An ansible role to install and configure helm.


Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`
```
Helm URL:
helm_url

Helm version:
helm_version

Helm platform:
helm_platform

Helm architecture:
helm_arch

Helm bin path:
helm_bin_path
```


Example Playbook
----------------
```
  - hosts: workstations
    roles:
      - role: helm
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
