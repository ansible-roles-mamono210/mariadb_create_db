[![CircleCI](https://circleci.com/gh/ansible-roles-mamono210/mariadb_create_db/tree/main.svg?style=svg)](https://circleci.com/gh/ansible-roles-mamono210/mariadb_create_db/tree/main)

Role Description
=========

Create [MariaDB](https://mariadb.org) database for CentOS Stream.

Requirements
------------

Before running this role, MariaDB server must be installed and running on the target system.

Role Variables
--------------

```YAML
mariadb_db_name: molecule
mariadb_db_password: molecule
mariadb_db_user: molecule
mariadb_root_password: password
```

Dependencies
------------

None

Example Playbook
----------------

```YAML
---
- hosts: all
  become: true
  roles:
    - mamono210.mariadb_install
    - mariadb_create_db
```

License
-------

BSD
