---
## Front matter
title: "Лабораторная работа №13"
subtitle: "Статистическая маршрутизация в Интернете. Планирование"
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

Провести подготовительные мероприятия по организации взаимодействия через сеть провайдера посредством статистической маршрутизации локальной сети сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в г. Сочи. 

# Выполнение лабораторной работы

1) Я внёс изменения в схемы L1, L2 и L3, добавив новые области: 42-й квартал и Сочи.

![Схема L1](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/2.jpg){#fig:001 width=70%}

![Cхема L2](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/1.jpg){#fig:002 width=70%}

![Cхема L3](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/3.jpg){#fig:003 width=70%}

2) В проекте разместил новое оборудование: 4 мадиаконвертора, 3 маршрутизатора, коммутатор и 3 оконечных устройства. Всем присвоил название. 

![Устройства в проекте](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/4.jpg){#fig:004 width=70%}

3) На медиаконверторах заменил модули, чтобы можно было подключить витую пару по оптоволокну и Fast Ethernet. 

![Замена модулей на медиаконверторах](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/5.jpg){#fig:005 width=70%}

4) На маршрутизаторе в 42-м квартале добавил дополнительный интерфейс.

![ДОП интерфейс на маршрутизаторе](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/6.jpg){#fig:006 width=70%}

5) В физическом пространстве добавил в Москве новое здание - 42 квартал и присвоил ему соответствующее имя.

![42-й квартал в физ области](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/7.jpg){#fig:007 width=70%}

6) В физическом пространстве добавил город Сочи.

![Сочи в физ области](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/8.jpg){#fig:008 width=70%}

7) Перенёс оборудование с Донской в город Сочи и здание 42-го квартала. 

![Оборудование 42 квартала](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/9.jpg){#fig:009 width=70%}

![Оборудование Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/10.jpg){#fig:010 width=70%}

8) Произвёл первоначальную настройку добавленного оборудования. 

![Маршрутизатор 1 в 42 квартале](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/11.jpg){#fig:011 width=70%}

![Коммутатор 1 в 42 квартале](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/12.jpg){#fig:012 width=70%}

![Маршрутизатор 2 в 42 квартале](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/13.jpg){#fig:013 width=70%}

![Коммутатор 2 в 42 квартале](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/14.jpg){#fig:014 width=70%}

![Маршрутизатор в Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/16.jpg){#fig:015 width=70%}

![Коммутатор в Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab13/report/image/15.jpg){#fig:016 width=70%}

# Выводы

Я провёл подготовительные мероприятия по организации взаимодействия через сеть провайдера посредством статистической маршрутизации локальной сети сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в Сочи. 
