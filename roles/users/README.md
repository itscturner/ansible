Users
=====

An Ansible role to manage users.

Requirements
------------

None.

Role Variables
--------------

The default values for the variables are set in defaults/main.yml:

| Variable                | Required | Default   | Choices                   | Comments                                                    |
|-------------------------|----------|-----------|---------------------------|-------------------------------------------------------------|
| users_manage            | no       |           |                           | Users to be managed by this role.                           |
| users_create_home       | yes      | true      | true, false               | Create home directories by default for users being created. |
| users_default_shell     | yes      | /bin/bash |                           | Default shell for users being created.                      |

Dependencies
------------

None.

Example Playbook
----------------

```
    - hosts: all
      roles:
         - role: users
           users_manage:
             - name: testuser1
               uid: 12345
             - name: testuser2
               state: absent
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
