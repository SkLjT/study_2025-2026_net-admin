---
## Front matter
title: "Лабораторная работа №16"
subtitle: "Настройка VPN"
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

Получение навыков настройки VPN-туннеля через незащищённое Интернет-соединение. 

# Выполнение лабораторной работы

1) Я разместил в рабочем проекте новую область - Пиза. Настроил медиаконверет для соединения между областями. 

![Настройка медиаконвертора](/home/aalushin1/study_2025-2026_net-admin/labs/lab16/report/image/1.jpg){#fig:001 width=70%}

![Схема проекта](/home/aalushin1/study_2025-2026_net-admin/labs/lab16/report/image/2.jpg){#fig:002 width=70%}

2) В физическом пространстве добавил ещё один город - Пиза. Переместил туда соответствующее оборудование.

![Здание Пиза](/home/aalushin1/study_2025-2026_net-admin/labs/lab16/report/image/3.jpg){#fig:003 width=70%}

3) Произвёл первоначальную настройку и настройку интерфейсов оборудования в Пизе. 

![Настройка маршрутизатора Пиза](/home/aalushin1/study_2025-2026_net-admin/labs/lab16/report/image/4.jpg){#fig:004 width=70%}

![Настройка коммутатора Пиза](/home/aalushin1/study_2025-2026_net-admin/labs/lab16/report/image/5.jpg){#fig:005 width=70%}

![Настройка интерфейсов маршрутизатора Пиза](/home/aalushin1/study_2025-2026_net-admin/labs/lab16/report/image/6.jpg){#fig:006 width=70%}

![Настройка интерфейсов коммутатора Пиза](/home/aalushin1/study_2025-2026_net-admin/labs/lab16/report/image/7.jpg){#fig:007 width=70%}

4) Настроил VPN на основе протокола GRE. 

![Настройка маршрутизатора Пиза](/home/aalushin1/study_2025-2026_net-admin/labs/lab16/report/image/9.jpg){#fig:008 width=70%}

![Настройка маршрутизатора Донская](/home/aalushin1/study_2025-2026_net-admin/labs/lab16/report/image/8.jpg){#fig:009 width=70%}

5) Проверил работоспособность VPN.

# Выводы

Я получил навыки настройки VPN-туннеля через незащищённое Интернет-соединение. 
