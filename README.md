# ДЗ: PostgreSQL с репликацией через Ansible

## Хосты
- Мастер: 192.168.88.162 (username/12345678)
- Реплика: 192.168.88.170 (pg-replica/12345678)

## Запуск
```bash
ansible-playbook -i hosts.ini deploy.yaml