# Домашнее задание к занятию «Система мониторинга Zabbix»- Николай Копосов

### Задание 1 

Установите Zabbix Server с веб-интерфейсом.

#### Процесс выполнения
1. Выполняя ДЗ, сверяйтесь с процессом отражённым в записи лекции.
2. Установите PostgreSQL. Для установки достаточна та версия, что есть в системном репозитороии Debian 11.
3. Пользуясь конфигуратором команд с официального сайта, составьте набор команд для установки последней версии Zabbix с поддержкой PostgreSQL и Apache.
4. Выполните все необходимые команды для установки Zabbix Server и Zabbix Web Server.

#### Требования к результаты 
1. Прикрепите в файл README.md скриншот авторизации в админке.
2. Приложите в файл README.md текст использованных команд в GitHub.

### Решение 1
1. ![login zabbix](/img/Screenshot%20at%20Oct%2026%2020-31-54.png)
2. - git clone git@github.com:koposow/zabbix_hw.git  
   - git remote set-url origin git@github.com:koposow/zabbix_hw.git
   - git config --global user.email nikolay@koposow.ru
   - git config --global user.name Nikolay Koposov
   - git status
   - git add . 
   - git commit -m 'First commit'
   - git push origin main
---

### Задание 2 

Установите Zabbix Agent на два хоста.

#### Процесс выполнения
1. Выполняя ДЗ, сверяйтесь с процессом отражённым в записи лекции.
2. Установите Zabbix Agent на 2 вирт.машины, одной из них может быть ваш Zabbix Server.
3. Добавьте Zabbix Server в список разрешенных серверов ваших Zabbix Agentов.
4. Добавьте Zabbix Agentов в раздел Configuration > Hosts вашего Zabbix Servera.
5. Проверьте, что в разделе Latest Data начали появляться данные с добавленных агентов.

#### Требования к результаты 
1. Приложите в файл README.md скриншот раздела Configuration > Hosts, где видно, что агенты подключены к серверу
2. Приложите в файл README.md скриншот лога zabbix agent, где видно, что он работает с сервером
3. Приложите в файл README.md скриншот раздела Monitoring > Latest data для обоих хостов, где видны поступающие от агентов данные.
4. Приложите в файл README.md текст использованных команд в GitHub

### Решение 2
1. ![conf_hosts](/img/conf_hosts.png)
2. ![agent_works](/img/agent_works.png)
3. ![wm_data](/img/vm1-2_data.png)
4. - git status
   - git add . 
   - git commit -m 'add agents'
   - git push origin main
---