[![](https://github.com/ansible-roles-mamono210/mariadb_create_db/workflows/build/badge.svg)](https://github.com/ansible-roles-mamono210/mariadb_create_db/actions?query=workflow%3Abuild)

Role Description
=========

Create [MariaDB](https://mariadb.org) database for CentOS7/Stream8.

Requirements
------------

Before running this role, MariaDB server ust be installed and running on the target system.

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
