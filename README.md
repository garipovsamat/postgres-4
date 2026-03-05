# PostgreSQL с репликацией

## Хосты
- Мастер: 192.168.88.162 (username / 12345678)
- Реплика: 192.168.88.172 (pg-replica / 12345678)

## Запуск
```bash
ansible-playbook -i inventory/hosts.ini deploy.yaml
```

Результаты на мастере
```bash
# pgbench
cat /tmp/pgbench_result.txt

# Медленные запросы
cat /tmp/slow_queries.txt

# IO запросы
cat /tmp/io_queries.txt

# Логи pgbench
sudo tail -50 /pg_data/16/log/postgresql-Thu.log | grep pgbench
```