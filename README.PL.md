Ansible.RoleSystem.SetHostname
=========

Ta rola ustawia nazwę hostname i edytuje wpis w pliku `/etc/config`

Język: [EN](README.md), [PL](README.PL.md)

Zmienne w roli
--------------
optional:
```
  inventory_fqdn: virtualmachine.local.net
```

Przykładowy Playbook
----------------

Przykładowe użycie roli
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

Testowane
------------

Testing on:
  - Ubuntu 16.04 LTS
  - Ubuntu 18.04 LTS
  - Ubuntu 20.04 LTS
  - Centos 7
  - Centos 8

Licencja
-------

BSD

Autor
------------------
 **Maciej Rachuna**
##### System Administrator & DevOps Engineer
rachuna.maciej@gmail.com