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

.. code-block:: yaml

  # The icingaweb2 web ui password
  icinga2_web_admin_pass: "passw0rd"
  
  # icinga2 API host
  icinga2_web_api_host: "127.0.0.1"
  
  # icinga2 API port
  icinga2_web_api_port: "5665"
  
  # icinga2 API user
  icinga2_web_api_user: "icingaweb2"
  
  # icinga2 API password
  icinga2_web_api_pass: "passw0rd"
  
  
  ## icingaweb2 database settings
  # The icingaweb2 database name
  icinga2_web_icingaweb2_database_name: "icingaweb2"
  
  # The icingaweb2 database user
  icinga2_web_icingaweb2_database_user: "icingaweb2"
  
  # The icingaweb2 database password
  icinga2_web_icingaweb2_database_pass: "passw0rd"
  
  # The icingaweb2 database host
  icinga2_web_icingaweb2_database_host: "127.0.0.1"
  
  # The icingaweb2 database port
  icinga2_web_icingaweb2_database_port: "3306"
  
  
  ## Icinga2 database settings
  # icinga2 database name
  icinga2_web_icinga2_database_name: "icinga2"
  #
  # icinga2 database host
  icinga2_web_icinga2_database_host: "127.0.0.1"
  
  # icinga2 database port
  icinga2_web_icinga2_database_port: "3306"
  
  # icinga2 database user
  icinga2_web_icinga2_database_user: "icinga2"
  
  # icinga2 database password
  icinga2_web_icinga2_database_pass: "passw0rd"


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
