aide
====

An ansible role to install and configure aide.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Aide database directory:
aide_db_dir

Aide database name:
aide_db

Aide new database name:
aide_db_new

Aide log directory:
aide_log_dir

Whether to gzip the output to database or not:
aide_gzip_dbout

Set how verbose aide is:
aide_verbose

The URL that the output is written to:
aide_report_url

List of aide rules:
aide_rules

List of aide cron jobs:
aide_cron_jobs
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: aide
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
