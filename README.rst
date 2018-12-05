================
ROLE ICINGA2_WEB
================

.. image:: https://img.shields.io/github/license/adfinis-sygroup/ansible-role-icinga2_web.svg?style=flat-square
  :target: https://github.com/adfinis-sygroup/ansible-role-icinga2_web/blob/master/LICENSE

.. image:: https://img.shields.io/travis/adfinis-sygroup/ansible-role-icinga2_web.svg?style=flat-square
  :target: https://travis-ci.org/adfinis-sygroup/ansible-role-icinga2_web

.. image:: https://img.shields.io/badge/galaxy-adfinis--sygroup.icinga2_web-660198.svg?style=flat-square
  :target: https://galaxy.ansible.com/adfinis-sygroup/icinga2_web

This role installs and configures icingaweb2.


Requirements
=============

What you will need to benefit from this role a webserver installed on the system.
At Adfinis, we use the following role:

* `adfinis-sygroup.nginx <https://galaxy.ansible.com/adfinis-sygroup/nginx>`_



Role Variables
===============

A description of the settable variables for this role should go here, including
any variables that are in defaults/main.yml, vars/main.yml, and any variables
that can/should be set via parameters to the role. Any variables that are read
from other roles and/or the global scope (ie. hostvars, group vars, etc.)
should be mentioned here as well.


Dependencies
=============

This role depends on the following roles:

* `adfinis-sygroup.php_fpm <https://galaxy.ansible.com/adfinis-sygroup/php_fpm>`_
* `adfinis-sygroup.icinga2_master <https://galaxy.ansible.com/adfinis-sygroup/icinga2_master>`_

Example Playbook
=================

.. code-block:: yaml

  - hosts: servers
    roles:
       - { role: adfinis-sygroup.icinga2_web }


License
========

`GPL-3.0 <https://github.com/adfinis-sygroup/ansible-role-icinga2_web/blob/master/LICENSE>`_


Author Information
===================

icinga2_web role was written by:

* Adfinis SyGroup AG | `Website <https://www.adfinis-sygroup.ch/>`_ | `Twitter <https://twitter.com/adfinissygroup>`_ | `GitHub <https://github.com/adfinis-sygroup>`_
