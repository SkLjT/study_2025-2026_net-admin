---
## Front matter
lang: ru-RU
title: Презентация по лабораторной работе 5
author:
  - Лушин А.А.
institute:
  - Российский университет дружбы народов, Москва, Россия
  - Факультет Физико-математических и естественных наук
date: 18 февраля 2005

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
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Лушин Артём Андреевич
  * Бакалавр направления компьютерные и информационные науки
  * Кафедра теории вероятности и кибербезопасности
  * Российский университет дружбы народов
  * [lusin5745@gmail.com](mailto:lusin5745@gmail.com)

:::
::: {.column width="30%"}

![](/home/aalushin1/cisco1/presentation/image/me.jpg)

:::
::::::::::::::

# Цели и задачи

## Цель

Получить основные навыки по настройке VLAN на коммутаторах сети. 

# Ход выполнения работы

## Настройка Trunk-портов

Используем последовательность команд, чтобы настроить trunk-порты на сооветствующих интерфейсах всех коммутаторов. Настраивали все коммутаторы: msk-donskaya-aalushin-sw-1, msk-donskaya-aalushin-sw-2, msk-donskaya-aalushin-sw-3, msk-donskaya-aalushin-sw-4, msk-pavlovskaya-aalushin-sw-1.

![](/home/aalushin1/lab5/presentation/image/2.jpg){#fig:001 width=70%}

## VTP-серве и VTP-клиент

Используя последовательность команд настроил коммутатор msk-donskaya-aalushin-sw-1, как VTP-сервер и прописал на нём номера и названия VLAN. Оставшиеся коммутаторы настроил как VTP-клиенты.

![](/home/aalushin1/lab5/presentation/image/6.jpg){#fig:002 width=70%}

## Выдача ip-адресов и шлюзов

На оконечных устройствах и серверах указываем статистические ip-адреса и шлюзы из плана ip-адресов. Важно для каждого устройства указать свой адрес.

![](/home/aalushin1/lab5/presentation/image/15.jpg){#fig:003 width=70%}

## Проверка работоспособности

С помощью команды ping проверяем доступность устройств, принадлежащих одному VLAN и недоступность устройств, принадлежащих разным VLAN. Затем в симуляции отправляем пакет ICMP и смотрим, чтобы не было ошибок. Анализируем содержание пакета. 

![](/home/aalushin1/lab5/presentation/image/24.jpg){#fig:004 width=70%}

# Результаты

## Выводы

Я получил основные навыки по настройке VLAN на коммутаторах сети. 
