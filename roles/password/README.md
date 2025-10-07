password
========

An ansible role to configure password policies.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Password quality file location:
password_complexity_file

Login definitions file location:
password_logindefs_file

Maximum number of days a password may be used:
password_passmaxdays

Minimum number of days allowed between password changes:
password_passmindays

Minimum acceptable password length:
password_passminlen

Number of days warning given before a password expires:
password_passwarnage

Number of characters in the new password that must not be present in the old password:
password_difok

Minimum acceptable size for the new password:
password_minlen

The maximum credit for having digits in the new password:
password_dcredit

The maximum credit for having uppercase characters in the new password:
password_ucredit

The maximum credit for having lowercase characters in the new password:
password_lcredit

The maximum credit for having other characters in the new password:
password_ocredit

The minimum number of required classes of characters for the new password (digits, uppercase, lowercase, others):
password_minclass

The maximum number of allowed consecutive same characters in the new password:
password_maxrepeat

The maximum number of allowed consecutive characters of the same class in the new password:
password_maxclassrepeat

Whether to check for the words from the passwd entry GECOS string of the user:
password_gecoscheck

Whether to check for the words from the cracklib dictionary:
password_dictcheck

Whether to check if it contains the user name in some form:
password_usercheck

Length of substrings from the username to check for in the password:
password_usersubstr

Whether the check is enforced by the PAM module and possibly other applications:
password_enforcing

Path to the cracklib dictionaries:
password_dictpath

Prompt user at most N times before returning with error:
password_retry

Enforces pwquality checks on the root user password:
password_enforceforroot

Skip testing the password quality for users that are not present in the /etc/passwd file:
password_localusersonly
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: password
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
