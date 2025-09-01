kubectl
=======

An ansible role to install kubectl.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Kubectl version:
kubectl_version

Kubectl URL:
kubectl_url

Validate certs when downloading kubectl:
kubectl_validate_certs

Kubectl bin path:
kubectl_bin_path
```

Example Playbook
----------------
```
  - hosts: workstations
    roles:
      - role: kubectl
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
