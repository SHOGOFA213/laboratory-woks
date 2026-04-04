---
## Front matter
lang: ru-RU
title: Администрирование локальных сетей
subtitle: Отчёт по лабораторной работе 8. Настройка сетевых сервисов. DHCP
author:
  - Абдуллахи Шугофа
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 6 April 2026

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

Освоить на практике механизм динамического назначения IP-адресов через протокол DHCP (Dynamic Host Configuration Protocol) в локальной вычислительной сети, а также получить навыки настройки DNS-сервера и его взаимодействия с DHCP.

## Построение топологии сети

![Топология сети](images/1.png)

## Настройка IP-адреса на DNS-сервере вручную

![Настройка IP-адреса DNS-сервера](images/2.png)

## Настройка DNS-службы на сервере

![Настройка IP-адреса DNS-сервера](images/3.png)

## Настройка DHCP на маршрутизаторе

![Настройка DHCP на маршрутизаторе](images/4.png)

## Получение IP-адресов клиентами по DHCP

![Получение IP-адресов клиентами по DHCP](images/5.png)

## Проверка сетевой доступности (связности)

![Проверка сетевой доступности ](images/11.png)

## Просмотр информации о пулах DHCP на маршрутизаторе

![Информация о пулах DHCP](images/12.png)

## Просмотр информации о пулах DHCP на маршрутизаторе

![Таблица выданных DHCP-адресов](images/13.png)

## Анализ процесса обмена DHCP-сообщениями в режиме симуляции
   
![DHCP Discover — исходное сообщение клиента](images/14.png)

## DHCP Offer 

![HCP Offer — предложение IP-адреса](images/16.png)

## DHCP Request 

![HCP Request — подтверждение выбора адреса](images/15.png)

## DHCP Acknowledgment (ACK) 
   
![DHCP ACK — подтверждение выдачи адреса](images/18.png)

## Процесс обмена DHCP-сообщениями в режиме симуляции

![Процесс обмена DHCP-сообщениями в режиме симуляции](images/17.png)

## Вывод

В ходе лабораторной работы был настроен DNS-сервер и созданы A-записи для четырёх доменных имён. На маршрутизаторе настроен DHCP-сервис с четырьмя пулами адресов для разных подсетей, клиенты успешно получили сетевые параметры автоматически. Проверка связности подтвердила корректную работу маршрутизации, а в режиме симуляции изучен полный процесс обмена DHCP-сообщениями (Discover, Offer, Request, ACK). Цель работы достигнута.

# Спасибо за внимание 
