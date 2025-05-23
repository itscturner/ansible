Users
=========

An Ansible role to manage users.

Example Playbook
----------------

```
---
    - hosts: all
      roles:
         - users
           users:
             # Add a user.
             - name: cturner
               comment: itscturner
               uid: 1234
               group: cturner
               groups:
                 - users
                 - wheel
                sudo_options: "ALL=(ALL) NOPASSWD: ALL"
                authorized_keys:
                  - "ssh-rsa CT12345"
                expires: -1
              # Remove a user.
              - name: removed_user
                state: absent
```

License
-------

Apache-2.0

Author Information
------------------

CTurner
