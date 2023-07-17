User
=========

Создание пользователя, присвоение ему sudo прав и добавление SSH ключа.

Role Variables
--------------

*new_user_name* – имя нового пользователя
*new_user_shell* – оболочка, назначаемая пользователю
*new_user_password* – пароль нового пользователя


Example Playbook
----------------

    - hosts: all
      roles:
         - user
