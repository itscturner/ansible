git
===

An ansible role to install and configure git.

Requirements
------------

None.

Role Variables
--------------
```
List of packages to install for git:
git_packages

List of users to configure for git:
git_users

Username of git user on system:
system_username

Name of git user:
git_user_name

Email of git user:
git_user_email

Username of git user:
git_username
```

Dependencies
------------

None.

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: git
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
