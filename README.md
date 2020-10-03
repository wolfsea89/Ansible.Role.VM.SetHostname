Ansible.RoleSystem.SetHostname
=========

This role sets the hostname and edits an entry in `/ etc / config`

Language: [EN](README.md), [PL](README.PL.md)

Role Variables
--------------
optional:
```
  inventory_fqdn: virtualmachine.local.net
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- hosts: localhost
  remote_user: root
  become: true
  gather_facts: yes
  roles:
    - role: set-hostname
      vars:
        inventory_fqdn: "{{ inventory_hostname }}.localdomain"
```

Testing
------------

Testing on:
  - Ubuntu 16.04 LTS
  - Ubuntu 18.04 LTS
  - Ubuntu 20.04 LTS
  - Centos 7
  - Centos 8

License
-------

BSD

Author Information
------------------
 **Maciej Rachuna**
##### System Administrator & DevOps Engineer
rachuna.maciej@gmail.com