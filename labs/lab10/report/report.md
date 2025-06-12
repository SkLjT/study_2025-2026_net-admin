---
## Front matter
title: "Лабораторная работа №10"
subtitle: "Настройка списков управления доступом (ACL)"
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

Освоить настройку прав доступа пользователей к ресурсам сети. 

# Выполнение лабораторной работы

1) В рабочей области проекта подключил ноутбук администратора к сети, чтобы резрешить ему потом любые действия, связанные с управлением сетью. 

![Размещение ноутбука администратора](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/1.jpg){#fig:001 width=70%}

![Конфигурация ноутбука](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/2.jpg){#fig:002 width=70%}

![Конфигурация ноутбука](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/3.jpg){#fig:003 width=70%}

2) Настроил доступ к web-серверу по протоколу tcp 80. 

![Настройка доступа к web](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/4.jpg){#fig:004 width=70%}

3) Добавил список управления доступом к интерфейсу.

![Добавление списка управления доступом](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/5.jpg){#fig:005 width=70%}

4) Настроил дополнительный доступ для администратора по протоколам telnet и ftp. 

![ДОП доступ по протоколам](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/6.jpg){#fig:006 width=70%}

5) Убедился, что с узла 10.128.6.200 есть доступ по протоколу FTP.

![Доступ по протоколу](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/7.jpg){#fig:007 width=70%}

6) Попробовал провести такую же процедуру с другого устройства сети. Увидел, что доступ запрещён.

![Доступ по протоколу](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/8.jpg){#fig:008 width=70%}

7) Настроил доступ к файловым серверам.

![Доступ к файловому серверу](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/9.jpg){#fig:009 width=70%}

8) Настроил доступ к почтовому серверу. 

![Доступ к почтовому серверу](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/10.jpg){#fig:010 width=70%}

9) Настроил доступ к DNS-серверу. 

![Доступ к DNS](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/11.jpg){#fig:011 width=70%}

10) Проверил работоспособность web сервера по ip-адресу и по имени сайта.

![web по ip-адресу](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/12.jpg){#fig:012 width=70%}

![web по имени](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/13.jpg){#fig:013 width=70%}

11) Настроил разрешение на icmp-запросы.

![Разрешение icmp](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/14.jpg){#fig:014 width=70%}

12) Посмотрел номера строк правил в списке контроля. 

![Список контроля](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/15.jpg){#fig:015 width=70%}

13) Настроил доступ для сети Other. 

![Доступ для other](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/16.jpg){#fig:016 width=70%}

14) Настроил доступ к сети сетевого оборудования.

![Доступ к сети оборудования](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/17.jpg){#fig:017 width=70%}

15) Проверил установленные правила доступа, попытавшись получить доступ по различным протоколам с разных устройств. Пропинговать сервера получилось со всех устройств, а вот сетевое оборудование только с admin.

![проверка с dep](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/18.jpg){#fig:018 width=70%}

![проверка с dk](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/19.jpg){#fig:019 width=70%}

![проверка с admin](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/20.jpg){#fig:020 width=70%}

16) Разрешил администратору из сети Other действия, аналогичные действиям администратора из другой сети. 

![Ноутбук администратора на повловской](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/21.jpg){#fig:021 width=70%}
 
![Права доступа администратора на повловской](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/22.jpg){#fig:022 width=70%}

17) Проверил корректность установленных правил доступа.

![Проверка с администратора павловской](/home/aalushin1/study_2025-2026_net-admin/labs/lab10/report/image/23.jpg){#fig:023 width=70%}

# Выводы

Я освоил настройку прав доступа пользователей к ресурсам сети. 


