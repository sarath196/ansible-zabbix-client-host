Role Name
=========
**ansible-zabbix-client-host**

simple zabbix-client setup configuration with Ansible Playbook,
This is simple lightweight configuration repository will contain all setup's and needed to correctly configure a Zabbix Client source
Requirements
------------
Operating systems
-----------------
- Red Hat

Zabbix Version
--------------
Default **zabbix release 3.4**
Also change zabbix release version in default variable file 
zabbix_repo_package : ['https://repo.zabbix.com/zabbix/4.0/rhel/7/x86_64/zabbix-release-4.0-1.el7.noarch.rpm']

Installation
------------
Use **runsetup.yml** file as host filerun playbook
```sh
$ ansible-playbook /path/runsetup.yml -i /path/inventory.txt
```
Role Variables
--------------

| Variables | Descriptions   |
|----------------|-------------------------------|
| zabbix_repo_package | zabbix dependency variables   |



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

This is my first attempt to create an ansible role, so please send suggestion or pull requests to make this role better.

Github: https://github.com/sarath196/ansible-zabbix-server-host
Mail: ksarath196@gmail.com
