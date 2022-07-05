1. Скопировать репозитарий к себе на машину
2. Зайти в скачанную папку 'Ansible'
3. Поднять управляемый хост: vagrant up
4. Проверить доступ к хосту: ansible nginx -m ping
5. Проверить статус firewalld (должен быть inactive): ansible nginx -m systemd -a name=firewalld
6. Установить nginx на хост с помощью playbook-файла: ansible-playbook nginx.yml
7. Убедиться в установке nginx: curl localhost
