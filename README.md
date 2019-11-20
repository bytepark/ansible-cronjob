[![Build Status](https://travis-ci.org/bytepark/ansible-cronjob.svg?branch=master)](https://travis-ci.org/bytepark/ansible-cronjob)

ansible-cronjob
=========

Ansible role to install and configure cronjobs

Requirements
------------

No further requirements besides bash.

Role Variables
--------------
Variables to use

```
# define list of cronjobs
#
# cronjobs:
# - name: 'Example cronjob'
#   user: 'root'
#   state: 'present'
#   minute: '20'
#   hour: '*'
#   day: '*'
#   weekday: '*'
#   month: '*'
#   job: 'curl www.google.com'
#   special_time: 'daily'

cronjobs: []
```

If `special_time` is set, `minute`, `hour`, `day`, `weekday` and `month` are ignored.

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

bytepark / 2019.
