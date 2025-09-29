facts
=====

An ansible role for creating custom facts.

```
You can pass key value pair to this role, which will place the facts in
`custom.fact`. For example this dictionary:

facts:
  - key: machine_type
    value: server
  - key: availability_zone
    value: west

Would make these facts available:

        "ansible_local": {
            "custom": {
                "machine_type": "server",
                "availability_zone": "west"
            }
        },
```

Role Variables
--------------

The default values for the variables are set in `defaults/main.yml`
```
Custom facts:
facts
```

Example Playbook
----------------
```
  - hosts: servers
    roles:
      - role: facts
        facts:
          - key: machine_type
            value: server
    
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
