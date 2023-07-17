nginx
=========

Установка Nginx и его настройка

Role Variables
--------------

*nginx_port* – порт, используемый сервером  nginx
*server_name* – название сервера
*document_root* – путь к директории хранения веб-приложений
*app_root* – название (путь) директории веб-приложения

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      handlers:
        - name: restart nginx
          become: yes
          service: name=nginx state=restarted
      roles:
         - nginx
