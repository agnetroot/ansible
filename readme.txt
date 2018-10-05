Сгенерируем SSH public key на ансибл сервере, если нужно
 
ssh-keygen -t rsa



Закинем ключик на удаленную машину 

ssh-copy-id raj@192.168.12.7



Проверим, можно ли уже зайти 

ssh raj@192.168.12.7



Выполним плейбук

ansible-playbook centos_deploy.yml
