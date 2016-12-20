[![Build Status](https://travis-ci.org/adamham/php-fpm.svg?branch=master)](https://travis-ci.org/adamham/php-fpm)

php-fpm
=========

Installs php-fpm and creates a listener pool. Useful for development but not
production ready.
For RHEL/CentOS/Debian/Ubuntu

Tested using Ansible 2.1.2 on:

CentOS 7
Debian Jessie
Ubuntu Trusty

Requirements
------------

Ansible 2+

Role Variables
--------------

vars/rhel-conf.yml and vars/deb-conf.yml containt OS specific settings to make
life easier (the package names differ slightly between them)

See templates/php-fpm.conf.j2 for an in depth explanation of all the global
variable settings

Useful links
------------

[ PHP: FPM configuration directives ](http://php.net/manual/en/install.fpm.configuration.php)

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      become: true
      roles:
         - php-fpm

License
-------

MIT
