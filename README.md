ansible-cronjob
=========

Ansible role to install and configure cronjobs

Requirements
------------

No further requirements besides bash.

Role Variables
--------------
Variable defaults

```
# list of cronjobs
#- { name: 'Example cronjob', minute: '20', hour: '*', job: 'curl www.google.com' }

cronjobs: []

```

Dependencies
------------

No dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: bytepark.cronjob }

License
-------

MIT

Author Information
------------------

bytepark / 2018.
