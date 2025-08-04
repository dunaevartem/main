### Команда для установки  
sudo ansible-playbook -i inventoy.ini install_docker.yaml --ask-become-pass  
### Команда для удаления  
sudo ansible-playbook -i inventory.ini remove_docker.yaml --ask-become-pass  
  
### Для установки требуется пробросить публичный ключ на серверы  
ssh-keygen -t rsa -b 2048 #создаем публичный ключ  
ssh-copy-id username@your_server #копируем на серверы  
### в моем случае:  
ssh-copy-id testing@192.168.1.51 && ssh-copy-id testing@192.168.1.52 && ssh-copy-id testing@192.168.1.53
