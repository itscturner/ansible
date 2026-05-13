Git
===

An Ansible role to install and configure Git.

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`

| Variable                   | Required | Default                  | Choices | Comments                                                              |
|----------------------------|----------|--------------------------|---------|-----------------------------------------------------------------------|
| git_user                   | yes      |                          |         | System username for the user.                                         |
| git_group                  | yes      |                          |         | System group for the user.                                            |
| git_username               | no       |                          |         | Git username of user.                                                 |
| git_user_email             | no       |                          |         | Git email of user.                                                    |
| git_repository_destination | yes      | /home/{{ git_user }}/git |         | Location to place the copies of the Git repositories that are cloned. |
| git_repositories           | no       |                          |         | Git Repositories to checkout. (Repository, Destination).              |

Example Playbook
----------------

```
    - hosts: workstations
      roles:
         - role: git
           git_user: cturner
           git_group: cturner
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
