# Домашнее задание к занятию 2 «Кластеризация и балансировка нагрузки» - `Иншаков Владимир`

---

### Задание 1
- Запустите два simple python сервера на своей виртуальной машине на разных портах
- Установите и настройте HAProxy, воспользуйтесь материалами к лекции по [ссылке](2/)
- Настройте балансировку Round-robin на 4 уровне.
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

---

### Решение 1

Скриншоты:

![Screen1](https://github.com/MrVanG0gh/Netology_sflt_02/blob/main/screens/Screen1_1.png)
Наглядная работа балансировщика на L4
![Screen2](https://github.com/MrVanG0gh/Netology_sflt_02/blob/main/screens/Screen1_2.png)
Статистика Haproxy, отражающая балансировку на 4-ом уровне

Файл с настройками haproxy:
[.cfg file](https://github.com/MrVanG0gh/Netology_sflt_02/blob/main/files/haproxy_ex1.cfg)


---

### Задание 2
- Запустите три simple python сервера на своей виртуальной машине на разных портах
- Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
- HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

---

### Решение 2

![Screen1](https://github.com/MrVanG0gh/Netology_sflt_02/blob/main/screens/Screen2_1.png)
Демонстрация работы балансировщика на L7
![Screen2](https://github.com/MrVanG0gh/Netology_sflt_02/blob/main/screens/Screen2_2.png)
Статистика Haproxy, отражающая балансировку на 7-ом уровне

Файл с настройками haproxy:
[.cfg file](https://github.com/MrVanG0gh/Netology_sflt_02/blob/main/files/haproxy_ex2.cfg)
