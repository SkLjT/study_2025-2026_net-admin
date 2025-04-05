---
## Front matter
title: "Лабораторная работа №5"
subtitle: "Конфигурирование vlan"
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

Получить основные навыки по настройке Vlan на коммутаторах сети. 

# Выполнение лабораторной работы

1) Используя приведённую ниже последовательность команд, настроил Trunk-порты на соответствующих интерфейсах всех коммутаторов.

![Trunk-порт на msk-donskaya-aalushin-sw-1](/home/aalushin1/lab5/report/image/1.jpg){#fig:001 width=70%}

![Trunk-порт на msk-donskaya-aalushin-sw-2](/home/aalushin1/lab5/report/image/2.jpg){#fig:002 width=70%}

![Trunk-порт на msk-donskaya-aalushin-sw-3](/home/aalushin1/lab5/report/image/3.jpg){#fig:003 width=70%}

![Trunk-порт на msk-donskaya-aalushin-sw-4](/home/aalushin1/lab5/report/image/4.jpg){#fig:004 width=70%}

![Trunk-порт на msk-pavlovskaya-aalushin-sw-1](/home/aalushin1/lab5/report/image/5.jpg){#fig:005 width=70%}

2) Используя приведённую ниже последовательность команд по конфигурировации VLAN, настроил коммутатор msk-donskaya-aalushin-sw-1 как VTP-сервер и прописал на нём номер и название VLAN.

![msk-donskaya-aalushin-sw-1 как VLAN](/home/aalushin1/lab5/report/image/6.jpg){#fig:006 width=70%}

3) Используя приведённую ниже последовательность команд по конфигурации диапазонов портов, настроил msk-donskaya-aalushin-sw-2 - msk-donskaya-aalushin-sw-4, msk-pavlovskaya-aalushin-sw-1 как VTP-клиенты и на интерфейсах указал принадлежность к VLAN.

![msk-donskaya-aalushin-sw-2 как VTP-клиента](/home/aalushin1/lab5/report/image/7.jpg){#fig:007 width=70%}

![msk-donskaya-aalushin-sw-3 как VTP-клиента](/home/aalushin1/lab5/report/image/8.jpg){#fig:008 width=70%}

![msk-donskaya-aalushin-sw-4 как VTP-клиента](/home/aalushin1/lab5/report/image/9.jpg){#fig:009 width=70%}

![msk-pavlovskaya-aalushin-sw-1 как VTP-клиента](/home/aalushin1/lab5/report/image/10.jpg){#fig:010 width=70%}

4) Указал статистические ip-адреса на оконечных устройствах и серверах. 

![Шлюз для серверов](/home/aalushin1/lab5/report/image/11.jpg){#fig:011 width=70%}

![IP-адрес для web](/home/aalushin1/lab5/report/image/12.jpg){#fig:012 width=70%}

![IP-адрес для file](/home/aalushin1/lab5/report/image/13.jpg){#fig:013 width=70%}

![IP-адрес для mail](/home/aalushin1/lab5/report/image/14.jpg){#fig:014 width=70%}

![Шлюз для ДК](/home/aalushin1/lab5/report/image/15.jpg){#fig:015 width=70%}

![IP-адрес для ДК](/home/aalushin1/lab5/report/image/16.jpg){#fig:016 width=70%}

![Шлюз для кафедры](/home/aalushin1/lab5/report/image/17.jpg){#fig:017 width=70%}

![IP-адрес для кафедры](/home/aalushin1/lab5/report/image/18.jpg){#fig:018 width=70%}

![Шлюз для администрации](/home/aalushin1/lab5/report/image/19.jpg){#fig:019 width=70%}

![IP-адрес для администрации](/home/aalushin1/lab5/report/image/20.jpg){#fig:020 width=70%}

![Шлюз для других пользователей](/home/aalushin1/lab5/report/image/21.jpg){#fig:021 width=70%}

![IP-адрес для других пользователей](/home/aalushin1/lab5/report/image/22.jpg){#fig:022 width=70%}

5) Проверил с помощью команды ping доступность устройств.

![Проверка пингом](/home/aalushin1/lab5/report/image/23.jpg){#fig:023 width=70%}

6) Изучил процесс передвижения пакета icmp по сети. Изучил содержимое пакета и заголовки протоколов. 

![Передвижение пакета](/home/aalushin1/lab5/report/image/24.jpg){#fig:024 width=70%}

![Содержание пакета](/home/aalushin1/lab5/report/image/25.jpg){#fig:025 width=70%}

# Выводы

Я получил основные навыки по настройке vlan на коммутаторах сети.  



















