---
## Front matter
title: "Лабораторная работа №9"
subtitle: "Использование протокола STP. Агрегирование каналов"
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

Изучение возможностей протокола STP и его модификаций по обеспечению отказоустойчивости сети, агрегированию интерфейсов и перераспределени  нагрузки между ними.

# Выполнение лабораторной работы

1) Сформировал резервное соединение между коммутаторами 1 и 3. Для этого заменил соединение между коммутаторами. 

![Логическая схема локальной сети с резеврвным соединением](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/1.jpg){#fig:001 width=70%}

![Активация портов в транковом режиме](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/2.jpg){#fig:002 width=70%}

![Активация портов в транковом режиме](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/3.jpg){#fig:003 width=70%}

![Активация портов в транковом режиме](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/4.jpg){#fig:004 width=70%}

2) С оконечного устройства dk-donskaya-1 пропинговал серверы mail u web. В режиме симуляции проследил движение пакета ICMP. Убедился, что движение пакетов происходит через коммутатор msk-donskaya-sw-2. 

![Пингование](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/5.jpg){#fig:005 width=70%}

![Симуляция](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/6.jpg){#fig:006 width=70%}

3) На коммутаторе msk-donskaya-sw-2 посмотрел состояние протокола STP.

![Информация о протоколе](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/7.jpg){#fig:007 width=70%}

4) В качестве корневого коммутатора STP настроил коммутатор msk-donskaya-sw-1.

![Настройка корневого коммутатора](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/8.jpg){#fig:008 width=70%}

5) Используя режим симуляции убедился, что пакеты ICMP пойдут от хоста до мейла через коммутаторы. 

![Симуляция](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/9.jpg){#fig:009 width=70%}

6) Настроил режим Postfax на тех интерфейсах коммтутаторов, к которым подключены серверы.

![Настройка режима Postfax](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/10.jpg){#fig:010 width=70%}

![Настройка режима Postfaх](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/11.jpg){#fig:011 width=70%}

7) Изучил отказоустойчивость протокола STP и время восстановления соединения при переключении на резервное соединение. 

![Пингование](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/12.jpg){#fig:012 width=70%}

8) Переключил коммутаторы режим работы на протокол Rapid PVST+.

![Режим работы по протоколу Rapid PVST+](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/13.jpg){#fig:013 width=70%}

![Режим работы по протоколу Rapid PVST+](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/14.jpg){#fig:014 width=70%}

![Режим работы по протоколу Rapid PVST+](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/15.jpg){#fig:015 width=70%}

![Режим работы по протоколу Rapid PVST+](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/16.jpg){#fig:016 width=70%}

9) Изучил отказоустойчивость протокола Режим Rapid PVST+ и врем восстановления соединения при подключении на резервное соединении. 

![Пингование](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/17.jpg){#fig:018 width=70%}

10) Сформировал агрегированное соединение.

![Логическая схема локальной сети с агрегированным соединением](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/18.jpg){#fig:019 width=70%}

11) Настроил агрегированное соединение. 

![Настройка агрегирования каналов](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/19.jpg){#fig:020 width=70%}

![Настройка агрегирования каналов](/home/aalushin1/study_2025-2026_net-admin/labs/lab9/report/image/20.jpg){#fig:021 width=70%}

# Выводы


Я изучил возможность протокола STP и его модификации по обеспечению отказоустойчивости сети, агрегированию интерфейсов и перераспределению нагрузки между ними. 







