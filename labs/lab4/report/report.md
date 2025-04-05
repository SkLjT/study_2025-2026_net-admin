---
## Front matter
title: "Лабораторная работа №4"
subtitle: "Первоначальное конфигурирование сети"
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

Провести подготовительную работу по первоначальной настройке коммутаторов сети. 

# Выполнение лабораторной работы

1) В рабочей области разместили коммутаторы и оконечные устройства согласно схеме L1 (lab3) и соединили их через соответствующие интерфейсы, используя прямые и кросс кабели. 

![Создание топологии](/home/aalushin1/lab4/report/image/1.jpg){#fig:001 width=70%}

2) Используя типовую конфигурацию коммутатора, настроили все коммутаторы, изменяя название устройств, ip-адреса согласно плану IP(lab3), устанавливая пароли и настраивая подключение по ssh. Настройка всех коммутаторов происходит абсолютно идентично, меняется только имя и ip-адрес. 

![Настройка msk-donskaya-aalushin-sw-1](/home/aalushin1/lab4/report/image/2.jpg){#fig:002 width=70%}

![Настройка msk-donskaya-aalushin-sw-2](/home/aalushin1/lab4/report/image/3.jpg){#fig:003 width=70%}

![Настройка msk-donskaya-aalushin-sw-3](/home/aalushin1/lab4/report/image/4.jpg){#fig:004 width=70%}

![Настройка msk-donskaya-aalushin-sw-4](/home/aalushin1/lab4/report/image/5.jpg){#fig:005 width=70%}

![Настройка msk-pavlovskaya-aalushin-sw-1](/home/aalushin1/lab4/report/image/6.jpg){#fig:006 width=70%}

# Выводы

Я провёл подготовительную работу по первоначальной настройке коммутаторов сети. 



















