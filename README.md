# Ansible Role for MySQL Community Server 8.0

![Build Status](https://github.com/6nsh/ansible-role-mysql_server/actions/workflows/ansible-galaxy-ci.yml/badge.svg)

This role helps to install and configure MySQL Community Server 8.0 to Debian (buster/bullseye).

Requirements
------------

This role requires Ansible 2.9 or higher.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows:

```yaml
    mysql_root_password: Aver@gEStr0ngPaSSw0rd
    mysql_data_dir: /path/to/mysql/data
    mysql_bind_address: 10.0.0.1
```

Variables 'mysql_data_dir' and 'mysql_bind_address' are optional.
Default values for optional variables:

```yaml
    mysql_data_dir: /var/lib/mysql
    mysql_bind_address: 127.0.0.1
```
Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      roles:
         - { role: 6nsh.mysql_server, tags: mysql_server }
```
License
-------

MIT

Author Information
------------------

This role was created by Artem Kasianchuk.
