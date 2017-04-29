Debian-Common
=============

Provides minimum updates for debian system

Requirements
------------

This role requires a debian compliant system such as knoppix or ubuntu.

Role Variables
--------------

debian:
    version: wheezy (Debian release name such as wheezy, jessie, etc...)

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-common, debian.version: wheezy }

Tasks
-----

  - Register [dotdeb](http://www.dotdeb.org/) gpg key
  - User [french debian mirrors](ftp://ftp.fr.debian.org/)
  - Update and upgrade system
  - Install [vim](http://www.vim.org/)
  - Install [curl](http://curl.haxx.se/)
  - Install [python-pycurl](http://pycurl.sourceforge.net/) (for ansible uses)
  - Install [gnugpg](http://www.gnupg.org/)
  - Install [rsync](http://rsync.samba.org/)
  - Install [wget](https://www.gnu.org/software/wget/)
  - Install [ack-grep](http://beyondgrep.com/)

License
-------

BSD
