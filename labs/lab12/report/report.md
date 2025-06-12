---
## Front matter
title: "Лабораторная работа №12"
subtitle: "Настройка NAT"
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

Приобрести практические навыки по настройке доступа локальной сети к внешней сети по средствам NAT. 

# Выполнение лабораторной работы

1) Я сделал первоначальную настройку маршрутизатора и коммутатора в сети провайдера. 

![Настройка маршрутизатора в провайдере](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/1.jpg){#fig:001 width=70%}

![Настройка коммутатора в провайдере](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/2.jpg){#fig:002 width=70%}

2) Настроил интерфейсы маршрутизатора и коммутатора на провайдерах.

![Настройка интерфейса маршрутизатора](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/3.jpg){#fig:003 width=70%}

![Настройка интерфейса коммутатора](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/4.jpg){#fig:004 width=70%}

3) Настроил интерфейсы маршрутизатора сети Донская для доступа к сети провайдера.

![Интерфейса маршрутизатора Донская](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/5.jpg){#fig:005 width=70%}

4) Настроил на маршрутизаторе сети Донская NAT с правилами, указанными в лабораторной.

![Настройка адресов](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/6.jpg){#fig:006 width=70%}

![Настройка списка доступа (Кафедра)](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/8.jpg){#fig:008 width=70%}

![Настройка списка доступа (Администрация)](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/9.jpg){#fig:009 width=70%}

![Настройка списка доступа (Ноутбук админа)](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/10.jpg){#fig:010 width=70%}

5) Настроил NAT. 

![Настройка PAT](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/11.jpg){#fig:011 width=70%}

![Интерфейс для NAT](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/12.jpg){#fig:012 width=70%}

6) Настроил доступ из Интернета. 

![Доступ из интернет (WWW)](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/13.jpg){#fig:013 width=70%}

![Доступ из интернет (Файловый сервер)](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/14.jpg){#fig:014 width=70%}

![Доступ из интернет (Почтовый сервер)](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/15.jpg){#fig:015 width=70%}

![Доступ из интернет (Доступ по RDR)](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/15.jpg){#fig:016 width=70%}

7) Проверил работоспособность заданных настроек. 

![Проверка](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/16.jpg){#fig:017 width=70%}

![Проверка](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/17.jpg){#fig:018 width=70%}

![Проверка](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/18.jpg){#fig:019 width=70%}

![Проверка](/home/aalushin1/study_2025-2026_net-admin/labs/lab12/report/image/19.jpg){#fig:020 width=70%}

# Выводы

Я приобрёл практические навыки по настройке доступа локальной сети к внешней сети по средствам NAT. 
