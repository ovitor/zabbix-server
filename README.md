zabbix-server
=========

Installs Zabbix server with Nginx and PHP-FPM on debian based (tested on Ubuntu 20.04).

Requirements
------------

You need to install the following on ansible host and .

```
ansible-galaxy collection install community.general
```

Also install the package `psycopg2` from your distribution

Role Variables
--------------

The variables defined on this role are:

* `zabbix_timezone: "America/Fortaleza"`
* `zabbix_postgres_dbname:`
* `zabbix_postgres_host:`
* `zabbix_postgres_port:`
* `zabbix_postgres_user:`
* `zabbix_postgres_pass:`

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
- hosts: servers
  roles:
    - role: ovitor.zabbix-server
      vars:
        zabbix_postgres_dbname: postgres
        zabbix_postgres_host: localhost
        zabbix_postgres_port: 5432
        zabbix_postgres_user: postgres
```

License
-------

BSD
