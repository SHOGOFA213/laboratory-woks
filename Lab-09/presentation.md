---
## Front matter
lang: ru-RU
title: Администрирование локальных сетей
subtitle: Лабораторная работа № 9. Использование протокола STP. Агрегирование каналов
author:
  - Абдуллахи Шугофа
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 10 Апреля 2026

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


## 1.Цель работы

Изучение возможностей протокола STP и его модификаций по обеспечению отказоустойчивости сети, агрегированию интерфейсов и перераспределению нагрузки между ними.

## Изменение топологии и создание резервного соединения

![Топология сети с резервным соединением](images/1.jpg){#fig:1}

##  Проверка прохождения ICMP-пакетов

![Результат пинга с sabdullakhi-dk-donskaya-1](images/3.jpg)

## движение ICMP-пакетов

![Движение ICMP-пакетов через msk-donskaya-sabdullakhi-sw-2](images/4.jpg)

##

![Движение ICMP-пакетов через msk-donskaya-sabdullakhi-sw-4](images/5.jpg)

## Просмотр состояния протокола STP для VLAN 3

![Настройка msk-donskaya-sabdullakhi-sw-1 как корневого](images/7.jpg)


## Изменение маршрута ICMP-пакетов после смены корневого моста

![Топология sabdullakhi-mail](images/9.jpg)

##

![Топология sabdullakhi-web](images/8.jpg)

## Настройка режима PortFast на серверных портах

![Настройка PortFast на msk-donskaya-sabdullakhi-sw-2](images/10.jpg)

## Настройка PortFast на msk-donskaya-sabdullakhi-sw-3

![Настройка PortFast на msk-donskaya-sabdullakhi-sw-3](images/11.jpg)

## Проверка отказоустойчивости классического STP

![Проверка отказоустойчивости STP](images/12.jpg)

##  Перевод коммутаторов в режим Rapid PVST+

![Перевод sw-1 в режим Rapid PVST+](images/13.jpg){width=60%}

![Перевод sw-2 в режим Rapid PVST+](images/14.jpg){width=60%}

## Проверка отказоустойчивости Rapid PVST+

![Проверка работы сети при использовании Rapid PVST+](images/18.jpg)

## Настройка EtherChannel на коммутаторе msk-donskaya-sabdullakhi-sw-1

![Настройка EtherChannel на msk-donskaya-sabdullakhi-sw-1](images/19.jpg)

## Настройка EtherChannel на коммутаторе msk-donskaya-sabdullakhi-sw-4

![Настройка EtherChannel на msk-donskaya-sabdullakhi-sw-4](images/20.jpg)

## Сформированное агрегированное соединение между коммутаторами

![Сформированное агрегированное соединение между коммутаторами](images/21.jpg)

## Успешная проверка соединения после настройки EtherChannel


![Успешная проверка соединения после настройки EtherChannel](images/22.jpg)

## Вывод

В ходе работы организовано резервное соединение между sw-1 и sw-3. Изучен протокол STP, проведена смена корневого коммутатора. На серверных портах настроен PortFast. Классический STP восстанавливается за 30–50 с, Rapid PVST+ — за 1–3 с. Настроен EtherChannel между sw-1 и sw-4. Построена отказоустойчивая сеть с быстрым восстановлением.


# Спасибо за внимание 
