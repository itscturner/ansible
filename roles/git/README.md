Git
===

An Ansible role to install and configure Git.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`

| Variable                   | Required | Default                     | Choices | Comments                                                              |
|----------------------------|----------|-----------------------------|---------|-----------------------------------------------------------------------|
| git_user                   | yes      |                             |         | System username for the user.                                         |
| git_group                  | yes      |                             |         | System group for the user.                                            |
| git_username               | no       |                             |         | Git username of user.                                                 |
| git_user_email             | no       |                             |         | Git email of user.                                                    |
| git_repository_destination | yes      | /home/{{ git_user }}/git    |         | Location to place the copies of the Git repositories that are cloned. |
| git_repositories           | no       |                             |         | Git Repositories to checkout. (Repository, Destination).              |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

```
    - hosts: all
      roles:
         - role: git
```

License
-------

See license.md

Author Information
------------------

itscturner
