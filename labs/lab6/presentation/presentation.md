---
## Front matter
lang: ru-RU
title: Презентация по лабораторной работе 6
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

Настроить статистическую маршрутизацию VLAN в сети.  

# Ход выполнения работы

## Расширение топологии

В нашу топологию добавляем новый маршрутизатор CIsco 2811. Подключаем его к коммутатору msk-donskaya-aalushin-sw-1.

![](/home/aalushin1/lab6/presentation/image/1.jpg){#fig:001 width=70%}

## Настройка маршрутизатора

Используя последовательность команда, сконфигурировали маршрутизатор. Задали имя, пароль для доступа к консоли (2 вида), настроил удалённый доступ по ssh. С помощью последовательности команд на интерфейсе f0/0 настроил виртуальные интерфейсы. 

![](/home/aalushin1/lab6/presentation/image/2.jpg){#fig:002 width=70%}

## Проверка работоспособности

Чтобы убедиться в правильной настройке маршрутизатора и интерфейсов, отправили два пинга. Один был с одного vlan, второй с разных vlan. Также отправили пакеты ICMP для проверки работоспособности. Проанализировали содержание пакетов. 

![](/home/aalushin1/lab6/presentation/image/5.jpg){#fig:003 width=70%}

# Результаты

## Выводы

Я настроил статистическую маршрутизацию VLAN в сети. 
