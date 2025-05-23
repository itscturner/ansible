Users
=========

An ansible role to manage users.

Example Playbook
----------------

    - hosts: all
      roles:
         - users
             name: cturner
             state: present
             comment: itscturner
             uid: 1234
             group: cturner
             groups:
               - users
             expires: -1


License
-------

Apache-2.0

Author Information
------------------

CTurner
