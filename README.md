Sysctl
======

[![Build Status](https://api.travis-ci.org/azmelanar/ansible-sysctl.png)](https://travis-ci.org/azmelanar/ansible-sysctl) [![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-sysctl-blue.svg?style=flat)](https://galaxy.ansible.com/list#/roles/2601)

Role for manage sysctl rules.

Requirements
------------

Tested with Ansible 1.8.2

Role Variables
--------------

Sysctl parameters can be set as dictionary. Example:
 
     sysctl_rules:
       kernel.panic: 10
       vm.swappiness: 10
 
Error on setting non-existent sysctl keys might be ignored with:

     sysctl_ignore_errors: "yes"

Dependencies
------------

None

Example Playbook
----------------

Example of usage:

    - hosts: servers
      roles:
         - { role: azmelanar.sysctl }

License
-------

MIT

Feedback, improvements, bugs
----------------------------

Please use [issues](https://github.com/azmelanar/ansible-sysctl/issues).
