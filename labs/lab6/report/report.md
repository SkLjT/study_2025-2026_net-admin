---
## Front matter
title: "Лабораторная работа №6"
subtitle: "Статистическая маршрутизация vlan"
author: "Лушин Артём Андреевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: false # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Настроить статистическую маршрутизацию VLAN в сети. 

# Выполнение лабораторной работы

1) В проекте разместили маршрутизатор Cisco 2811, подключили к нему 24 коммутатора msk-donskaya-aalushin-sw-1.

![Топология](/home/aalushin1/lab6/report/image/1.jpg){#fig:001 width=70%}

2) Сконфигурировал маршрутизатор, задав на нём имя, пароль и настроил удалённое подключение по ssh.

![Конфигурация маршрутизатора](/home/aalushin1/lab6/report/image/2.jpg){#fig:002 width=70%}

3) Настроил порт 24 коммутатора msk-donskaya-aalushin-sw-1, как trunk-порт. 

![Настройка порта на коммутаторе](/home/aalushin1/lab6/report/image/3.jpg){#fig:003 width=70%}

4) На интерфейсе f0/0 маршрутизатора msk-donskaya-aalushin-gw-1 настроил виртуальные интерфейсы, соответствующие номерам VLAN. Согласно таблице IP-адресов задал соответствующие адреса на виртуальные интерфейсы. 

![Настройка интерфейсов маршрутизатора](/home/aalushin1/lab6/report/image/4.jpg){#fig:004 width=70%}

5) Проверил доступность оконечных устройств на разных VLAN. Сначала пропинговал dk-pavovskaya-aalushin-1 с dk-donskaya-aalushin-1, это один vlan. Затем пропинговал dk-pavovskaya-aalushin-1 с other-donskaya-aalushin-1, потому что они с разными vlan. 

![Пингование с одного vlan](/home/aalushin1/lab6/report/image/5.jpg){#fig:005 width=70%}

![Пингование с разных vlan](/home/aalushin1/lab6/report/image/6.jpg){#fig:006 width=70%}

6) В режиме симуляции запустил отправку пакетов ICMP и посмотрел что будет. Проанализировал содержимое пакета. 

![Отправка пакета](/home/aalushin1/lab6/report/image/7.jpg){#fig:007 width=70%}

![Содержимое пакета](/home/aalushin1/lab6/report/image/8.jpg){#fig:008 width=70%}

# Выводы

Я настроил статистическую маршрутизацию VLAn в сети. 


















