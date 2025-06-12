---
## Front matter
title: "Лабораторная работа №14"
subtitle: "Статистическая маршрутизация в Интернете. Настройка"
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

Настроить взаимодействие через сеть провайдера посредством статистической маршрутизации локальной сети организации с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в Сочи. 

# Выполнение лабораторной работы

1) Я настроил связь между территориями. 

![Настройка интерфейсов коммутатора провайдера](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/1.jpg){#fig:001 width=70%}

![Настройка интерфейсов маршрутизатора Донская](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/2.jpg){#fig:002 width=70%}

![Настройка интерфейсов маршрутизатора 1 42-квартал](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/3.jpg){#fig:003 width=70%}

![Настройка интерфейсов коммутатора Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/4.jpg){#fig:004 width=70%}

![Настройка интерфейсов маршрутизатора Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/5.jpg){#fig:005 width=70%}

2) Настроил оборудование, расположенное в 42-м квартале. 

![Настройка интерфейсов маршрутизатора 1 42-й квартал](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/6.jpg){#fig:006 width=70%}

![Настройка интерфейсов коммутатора 1 42-й квартал](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/7.jpg){#fig:007 width=70%}

![Настройка интерфейсов маршрутизатора 2 42-й квартал](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/8.jpg){#fig:008 width=70%}

![Настройка интерфейсов коммутатора 2 42-й квартал](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/9.jpg){#fig:009 width=70%}

3) Настроил оборудование, расположенное в Сочи. 

![Настройка интерфейсов маршрутизатора Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/10.jpg){#fig:010 width=70%}

![Настройка интерфейсов коммутатора Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/11.jpg){#fig:011 width=70%}

4) Настроил статистическую маршрутизацию между территориями. 

![Настройка маршрутизатора Донская](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/12.jpg){#fig:012 width=70%}

![Настройка маршрутизатора 1 42-й квартал](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/13.jpg){#fig:013 width=70%}

![Настройка маршрутизатора Сочи](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/14.jpg){#fig:014 width=70%}

5) Настроил статистическую маршрутизацию на территории 42-го квартала. 

![Настройка маршрутизатора 1 42-квартал](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/15.jpg){#fig:015 width=70%}

![Настройка интерфейсов маршрутизатора 2 42-квартал](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/16.jpg){#fig:016 width=70%}

6) Настроил NAT на маршрутизаторе Донская.

![NAT на маршрутизатора Донская](/home/aalushin1/study_2025-2026_net-admin/labs/lab14/report/image/17.jpg){#fig:017 width=70%}

# Выводы

Я настроил взаимодействие через сеть провайдера посредством статистической маршрутизации локальной сети организации с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в Сочи. 
