# TL;DR
./script {server1},{server2}

## Пример
./script 10.211.55.8,10.211.55.9

# Что делает скрипт?
Скрипт script генерирует инвентарь inventory.ini из 2 хостов согласно параметру, затем запускает playbook, который вычисляет загруженность серверов по метрике: cpu usage (%) - free RAM (%), выбирает из них менее загруженный в качестве целевого, устанавливает на целевой сервер и конфигурирует PostgreSQL и настраивает firewall.
