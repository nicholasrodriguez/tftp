tftp
====

This role is used by this repo [https://github.com/nicholasrodriguez/lab] to deploy tftp for an Ansible lab or test environment and will perform the following:

 - Install tftp
 - Configure tftp
 - Fix a CentOS 8 issue with tftp-server service start
 - Ensure firewalld is running and configured for tftp

Requirements
------------

Role tested on CentOS 7 and CentOS 8

Role Variables
--------------

| Variable                   | Default | Comments                                                                                                                                                  |
| :---                       | :---    | :---                                                                                                                                                      |
| `tftp_service`    | `tftp-service`      | |
| `tftp_root_directory`    | `/var/lib/tftpboot`      | |


Dependencies
------------

None required


Example Playbook
----------------

```
    - hosts: servers
      roles:
         - role: nicholasrodriguez.tftp
```
License
-------

MIT

Author Information
------------------

- https://github.com/nicholasrodriguez/ (maintainer)
