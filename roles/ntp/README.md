ntp
===

An ansible role to install and configure ntp.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
List of ntp packages:
ntp_packages

NTP service name:
ntp_service

NTP configuration file:
ntp_conf

List of IP Addresses to listen on:
ntp_interfaces

List of NTP pools:
ntp_pool

NTP Timezone:
ntp_timezone

NTP logging directory:
ntp_log_dir

Minimum number of selectable sources required to adjust the system clock:
ntp_min_sources
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: ntp
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
