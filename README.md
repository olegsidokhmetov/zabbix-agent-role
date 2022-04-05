Zabbix agent intsallation
=========

Role for instaling Zabbix agent

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

- Server IP with Zabbix
`ip_zabbix_server: 95.217.188.202`

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:



    ---
    
    - hosts: Zabbix-Agent
      gather_facts: true
      become: true 
      vars_files:
        - /etc/ansible/roles/zabbix-agent/defaults/main.yml
        - /etc/ansible/roles/zabbix-agent/vars/main.yml
    
      roles:
        - role: "/etc/ansible/roles/zabbix-agent"

License
-------

BSD

Author Information
------------------

Oleg Sidokhmetov
