Facts
=========

An Ansible role to configure custom facts.

Example Playbook
----------------

    - hosts: servers
      roles:
         - facts
           facts:
             - key: machine_type
               value: server

License
-------

Apache-2.0

Author Information
------------------

CTurner
