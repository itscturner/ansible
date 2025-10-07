users
=====

An ansible role to manage users.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Default shell for users:
users_shell

List of users:
users
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: users
          - name: cturner
            uid: 123456
            group: 123456
            groups: ["sudo", "wheel"]
            comment: "itscturner"
            home_create: true
            home: /home/cturner
            shell: /bin/zsh
          - name: user2
            state: absent
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
