Storage
=======

An Ansible role to create and manage partitions, volume groups, volumes, filesystems and mounts.

Role Variables
--------------
The default values for the variables are set in `defaults/main.yml`
```
Required packages for the storage role:
  storage_required_packages

Default options for Volume Groups:
  storage_volume_group_default_options

Default Filesystem type:
  storage_default_fstype

Partitions to configure (Name, Number, Flags - defaults to 'omit', Partition Start - defaults to 'omit', Partition End - defaults to 'omit', Label - defaults to 'omit'):
  storage_partition

Volume Groups to configure (Name, Devices, Size - defaults to 'omit', Options - defaults to 'storage_volume_group_default_options'):
  storage_volume_group

Volumes to configure (Name, VG, Size, Options - defaults to 'omit'):
  storage_volume

Filesystems to configure (Name, FSType - defaults to 'storage_default_fstype'):
  storage_filesystem

Mounts to configure (Name, Source, FSType - defaults to 'storage_default_fstype', Options - defaults to 'omit', Boot - defaults to 'omit', Dump - defaults to 'omit', PassNo - defaults to 'omit', Owner - defaults to 'omit', Group - defaults to 'omit', Mode - defaults to 'omit'):
  storage_mount
```

Example Playbook
----------------
```
  - hosts: all
    roles:
      - role: storage
```

License
-------

Apache-2.0

Author Information
------------------

itscturner
