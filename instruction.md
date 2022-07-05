1. Установить Ansible
2. Скопировать репозитарий к себе на машину
3. Зайти в скачанную папку 'Ansible'
4. Поднять управляемый хост: vagrant up
5. Проверить доступ к хосту: ansible nginx -m ping
6. Проверить статус firewalld (должен быть inactive): ansible nginx -m systemd -a name=firewalld
7. Установить nginx на хост с помощью playbook: ansible-playbook nginx.yml
8. Убедиться в установке nginx: curl localhost
