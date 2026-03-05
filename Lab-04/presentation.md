---
## Front matter
lang: ru-RU
title: Администрирование локальных сетей
subtitle: Лабораторная работа № 4. Первоначальное конфигурирование сети
author:
  - Абдуллахи Шугофа
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 03 марта 2026

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
Целью данной лабораторной работы является выполнение первоначальной
настройки сетевых коммутаторов в соответствии с заданной топологией L1. Под
первоначальной настройкой понимается:
присвоение устройству уникального имени; назначение IP адреса для управ-
ления устройством; настройка шлюза по умолчанию; конфигурирование пароль-
ной защиты на консольном порту и виртуальных терминалах (VTY); настройка
защищенного удаленного доступа по протоколу SSH.

## Построение топологии сети
Использованные коммутаторы:
- msk pavlovskaya sabdullakhi sw 1
- msk donskaya sabdullakhi sw 1
- msk donskaya sabdullakhi sw 2
- msk donskaya sabdullakhi sw 3
- msk donskaya sabdullakhi sw 4

![Построение топологии сети](images/1.jpg)

## Настройка msk donskaya sabdullakhi sw 1

![Настройка msk donskaya sabdullakhi sw 1](images/2.jpg)

##  Настройка msk donskaya sabdullakhi sw 2

![Настройка msk donskaya sabdullakhi sw 2](images/3.jpg)

##  Настройка msk donskaya sabdullakhi sw 3

![Настройка msk donskaya sabdullakhi sw 3](images/4.jpg)

## Настройка msk donskaya sabdullakhi sw 4

![Настройка msk donskaya sabdullakhi sw 4](images/5.jpg)

## Настройка msk pavlovskaya sabdullakhi sw 1

![Настройка msk pavlovskaya sabdullakhi sw 1](images/6.jpg)

## Заключение

В ходе лабораторной работы выполнено первоначальное конфигурирование пяти коммутаторов согласно схеме сети L1. Каждому устройству присвоено уникальное имя, назначен IP-адрес управления из подсети 10.128.1.0/24, настроен шлюз по умолчанию.

Реализована защита доступа: установлены пароли на console и VTY, настроен привилегированный режим, включено шифрование. Для безопасного удалённого управления на всех коммутаторах настроен доступ по SSH.

Все конфигурации сохранены. Коммутаторы готовы к удалённому администрированию.

# Спасибо за внимание 
