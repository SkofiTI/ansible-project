ssh_cfg
=========

Смена порта SSH и закрытие доступа по паролю

Role Variables
--------------

*ssh_port* – значение нового порта

Example Playbook
----------------

    - hosts: all
      handlers:
        - name: restart sshd
          become: yes
          service: name=ssh state=restarted
      roles:
        - ssh_cfg
