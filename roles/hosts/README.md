Hosts
=====

An Ansible role to manage the /etc/hosts and /etc/hostname files.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Hostname for /etc/hostname file:
  hosts_hostname

Entries to add to /etc/hosts file (Address, Hostnames):
  hosts_entries
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: hosts
        vars:
          hosts_entries:
            - address: 1.2.3.4
              hostnames:
                - server
                - server.example.com
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
