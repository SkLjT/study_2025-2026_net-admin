---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Планирование локальной сети организации"
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

Познакомиться с принципами планирование локальной сети организации. 

# Выполнение лабораторной работы

1) Используя графический редактор Dia, я повторил схемы L1, L2, L3. 

![Схема L1](/home/aalushin1/lab3/report/image/1.jpg){#fig:001 width=70%}

![Схема L2](/home/aalushin1/lab3/report/image/2.jpg){#fig:002 width=70%}

![Схема L3](/home/aalushin1/lab3/report/image/3.jpg){#fig:003 width=70%}

2) Повторил таблицу Vlan, IP-адресов и портов подключения оборудования планируемой сети. 

![Таблица vlan](/home/aalushin1/lab3/report/image/4.jpg){#fig:004 width=70%}

![Таблица IP-адресов](/home/aalushin1/lab3/report/image/5.jpg){#fig:005 width=70%}

![Таблица портов](/home/aalushin1/lab3/report/image/6.jpg){#fig:006 width=70%}

![Регламент выделения ip-адресов](/home/aalushin1/lab3/report/image/7.jpg){#fig:007 width=70%}

3) Сделал аналогичный план адресного пространства для сети 172.16.0.0/12 с соответствующими схемами сети и сопутствующими таблицами Vlan, IP-адресов и портов подключения.

![Устройства сети с номерами портов L1](/home/aalushin1/lab3/report/image/8.jpg){#fig:008 width=70%}

![Схема vlan сети L2](/home/aalushin1/lab3/report/image/9.jpg){#fig:009 width=70%}

![Схема маршрутизатора сети L3](/home/aalushin1/lab3/report/image/10.jpg){#fig:010 width=70%}

![Новая таблица IP](/home/aalushin1/lab3/report/image/12.jpg){#fig:011 width=70%}

![Новая таблица портов](/home/aalushin1/lab3/report/image/11.jpg){#fig:012 width=70%}

4) Сделали ещё один аналогичный план адресного пространства для сети 192.168.0.0/16 с соответсвующей схемой сети и сопутствующей таблицей IP-адресов.

![Заключительная таблица IP](/home/aalushin1/lab3/report/image/13.jpg){#fig:013 width=70%}

![Заключительная схема маршрутизации сети](/home/aalushin1/lab3/report/image/14.jpg){#fig:014 width=70%}

# Выводы

Я познакомился с принципами планирования локальной сети организации.



















