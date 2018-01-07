`mariadb` ansible role
======================

Description
-----------

Installs MariaDB on CentOS 7 and hardens it.

Official MariaDB yum repository is used <http://yum.mariadb.org/10.2/centos7-amd64>.

Presence of `/etc/mysql_hardened` file defines whether the hardening was applied.

Role Variables
--------------
Mandatory variable:

    mariadb_root_password

it doesn't have a default value so play would fail with error if this variable isn't defined

    mariadb_version

major version of Maria DB. By default it's a latest stable version 10.2.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: mariadb, mariadb_root_password: 'secret' }

License
-------

MIT
