---
## Front matter
title: "Лабораторная работа №15"
subtitle: "Динамическая маршрутизация"
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

Настроить динамическую маршрутизацию между территориями организации. 

# Выполнение лабораторной работы

1) Я настроил динамическую маршрутизацию по протоколу OSPF на маршрутизаторе Донская.

![Настройка маршрутизатора Донская](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/1.jpg){#fig:001 width=70%}

![Проверка OSPF на Донской](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/2.jpg){#fig:002 width=70%}

![Проверка OSPF на Донской](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/3.jpg){#fig:003 width=70%}

2) Я настроил динамическую маршрутизацию по протоколу OSPF на маршрутизаторе 1 42-го квартала.

![Настройка маршрутизатора 1 42-го квартала](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/4.jpg){#fig:004 width=70%}

3) Я настроил динамическую маршрутизацию по протоколу OSPF на маршрутизаторе 2 42-го квартала.

![Настройка маршрутизатора 2 42-го квартала](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/5.jpg){#fig:005 width=70%}

4) Настроил динамическую маршрутизацию по протоколу OSPF на маршрутизатора Сочи. 

![Настройка маршрутизатора Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/6.jpg){#fig:006 width=70%}

5) Я настроил связь между 42-м кварталом и Сочи напрямую. 

![Настройка интерфейса коммутатора Провайдера](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/7.jpg){#fig:007 width=70%}

![Настройка маршрутизатора 1 42-го квартала](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/8.jpg){#fig:008 width=70%}

![Настройка коммутатора Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/9.jpg){#fig:009 width=70%}

![Настройка маршрутизатора Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/10.jpg){#fig:010 width=70%}

6) В режиме симуляции отследил движение пакетов ICMP с ноутбука администратора на Донской, до компьютера пользователя в Сочи. Покет идёт через коммутаторы и маршрутизаторы на Донской, далее через медиаконверторы и коммутаторы на территории провайдера, а затем уже на коммутаторы и маршрутизаторы в Сочи. 

![Симуляция 1](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/11.jpg){#fig:011 width=70%}

7) На коммутаторе провайдера отключил временно vlan 6 и запустил пакет ICMP по тому же маршруту. Пакет пошёл через коммутаторы и маршрутизаторы на Донской, затем через медиаконверторы и коммутаторы на территории провайдера, оттуда на маршрутизатор на территории 42-го квартала, а уже оттуда в Сочи.

![Отключение vlan 6](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/12.jpg){#fig:012 width=70%}

![Симуляция 2](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/13.jpg){#fig:013 width=70%}

8) На коммутаторе провайдера снова включил vlan 6. Запустил пакет как и в предыдущих разах. Пакет пошёл также, как при первой симуляции. 

![Включение vlan 6](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/14.jpg){#fig:014 width=70%}

![Симуляция 3](/home/aalushin1/study_2025-2026_net-admin/labs/lab15/report/image/15.jpg){#fig:015 width=70%}

# Выводы

Я настроил динамическую маршрутизацию между территориями организации. 
