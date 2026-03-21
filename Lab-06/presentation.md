---
## Front matter
lang: ru-RU
title: Администрирование локальных сетей
subtitle: Лабораторная работа № 6. Статическая маршрутизация VLAN 
author:
  - Абдуллахи Шугофа
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 13 марта 2026

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
pdf-engine: xelatex

header-includes: |
  \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
  \usepackage{fontspec}
  \setmainfont{DejaVu Serif}
  \setsansfont{DejaVu Sans}
  \setmonofont{DejaVu Sans Mono}
---

## Цель работы

Настроить статическую маршрутизацию между виртуальными локальными сетями (VLAN) в среде Cisco Packet Tracer с использованием технологии RouteronaStick и провести анализ передачи данных между различными VLAN.

##  Построение топологии сети

![топологии сети](images/1.png){width=60%}


## Первичная настройка маршрутизатора

![Первичная настройка маршрутизатора через CLI](images/2.png){width=60%}

## Первичная настройка маршрутизатора
 
![Первичная настройка маршрутизатора через CLI](images/3.png){width=70%}
 

## Настройка межсетевой маршрутизации VLAN (RouteronaStick)

 ![Настройка VLANинтерфейсов маршрутизатора](images/4.png){width=70%}

## Проверка доступности устройств (ping)

 ![Проверка доступности узлов с помощью команды ping](images/5.png){width=80%}
 
## Дополнительно выполнена проверка

 ![Дополнительная проверка соединения между подсетями](images/6.png){width=70%}
 
## Анализ передачи данных в режиме Simulation

 ![Просмотр перемещения пакета в режиме Simulation](images/7.png){width=80%}
 
## Анализ передачи данных в режиме Simulation
 
 ![Просмотр перемещения пакета в режиме Simulation](images/8.png){width=70%}

 
## Анализ структуры передаваемого пакета

![Анализ структуры передаваемого ICMPпакета](images/9.png){width=80%}
 
## Вывод

В ходе лабораторной работы в Cisco Packet Tracer была построена сеть с маршрутизатором Cisco 2811, коммутаторами Cisco 2960, ПК и серверами. Маршрутизатор подключён к коммутатору через trunk-соединение для передачи трафика нескольких VLAN.

На маршрутизаторе выполнена базовая настройка (имя, пароли, SSH) и созданы виртуальные подинтерфейсы с IP-адресами для маршрутизации между VLAN.

Проверка командой ping подтвердила успешную передачу данных между VLAN. В режиме Simulation изучен процесс прохождения ICMP-пакета и структура кадров Ethernet, IP и ICMP.

# Спасибо за внимание 
