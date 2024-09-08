# linux-professional
Создается две машины. На одной устанавливает  ansible, на другой через ansible - nginx.
- Запустить vagrant up. 
- Запустить vagrant ssh ubuntu_ansible.
- Перейти в директори cd /opt/hosts. Из директории запустить следующие команды:
  - sudo ansible nginx -m ping
  - sudo ansible-playbook -vvv nginx.yaml
  - sudo curl http://192.168.11.150:8080