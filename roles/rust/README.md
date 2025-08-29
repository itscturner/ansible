rust
====

An ansible role to install and configure rust.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Where the rust installer will be downloaded to:
rust_installer_download_destination

Additional packages for rust:
rust_additional_packages
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: rust
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
