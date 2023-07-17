packages
=========

Обновление всех пакетов + установка mc, htop, atop, ncdu

Role Variables
--------------

*packages* – список, хранящий все нужные пакеты для установки

Example Playbook
----------------

    - hosts: all
      roles:
         - packages
