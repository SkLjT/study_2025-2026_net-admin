---
## Front matter
title: "Лабораторная работа №11"
subtitle: "Настройка NAT. Планирование"
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

Провести подготовительные мероприятия по подключению локальной сети организации к Интернет.

# Выполнение лабораторной работы

1) Я внёс изменения в схему L1 сети, добавив в неё сеть провайдера и сеть модельного интернета с указанием названий оборудования и портов подключения. 

![Схема L1](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/1.jpg){#fig:001 width=70%}

2) Я внёс соответвующие изменения в схему L2 и L3. Скорректировал таблицу распределения ip-адресов и портов.

![Схема L2](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/2.jpg){#fig:002 width=70%}

![Схема L3](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/3.jpg){#fig:003 width=70%}

![Таблица IP](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/5.jpg){#fig:004 width=70%}

![Таблица портов](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/4.jpg){#fig:005 width=70%}

3) В проекте разместил оборудование согласно схеме. То есть добавил 4 медиаконвертора, 2 коммутатора, маршрузатор и 4 сервера. Присвоил название размещённым в сети провайдера и сети интернета объектам. 

![Схема сети](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/6.jpg){#fig:006 width=70%}

4) На физическом уровне добавил здания провайдера и интернета в Москве. Присвоил им соответствующие названия. 

![Добавление на физ уровне](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/7.jpg){#fig:007 width=70%}

5) Перенёс из сети Донская оборудование в здание провайдера и интернета соответственно. 

![Перенос оборудования интернета](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/8.jpg){#fig:008 width=70%}
 
![Перенос оборудования провайдера](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/9.jpg){#fig:009 width=70%}

6) На медиаконверторах заменил модули согласно инструкции, чтобы можно было подключить витую пару по технологии Fast Ethernet и оптоволокну соответственно. 

![Модули медиаконвертора](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/10.jpg){#fig:010 width=70%}

7) Провёл соединение объектов согласно схеме.

![Соединение объектов](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/11.jpg){#fig:011 width=70%}

8) Прописал ip-адреса серверам. 

![Адрес шлюза](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/12.jpg){#fig:012 width=70%}

![ip-aдрес](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/13.jpg){#fig:013 width=70%}

9) Прописал сведения о серверах на dns-сервере. 

![записи на dns-сервере](/home/aalushin1/study_2025-2026_net-admin/labs/lab11/report/image/14.jpg){#fig:014 width=70%}

# Выводы

Я провёл подготовительные мероприятия по подключения локальной сети организации к Интернет. 

