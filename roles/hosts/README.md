hosts
=====

An ansible role to configure the hosts and hostname files.

Requirements
------------

None

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`
```
Hosts packages:
hosts_packages

Hostname. By default, this is set to whatever the inventory is set to.
hosts_hostname

Fully qualified domain name. By default, this is set to whatever the inventory is set to.
hosts_hostname_fqdn

Location of the hosts file:
hosts_file

Whether or not to reboot the host when the hostname is changed:
hosts_hostname_reboot
```

Dependencies
------------

None

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: hosts
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
