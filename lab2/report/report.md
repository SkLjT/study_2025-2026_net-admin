---
## Front matter
title: "Лабораторная работа №2"
subtitle: "Предварительное настройка оборудования Cisco"
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

Получить основные навыки по начальному конфигурированию оборудования Cisco.

# Выполнение лабораторной работы

1) В логической области разместили коммутатор, маршрутизатор и 2 оконечных устройства РС. Один РС соединили с коммутатором, второй с маршрутизатором.

![Создание топологии](/home/aalushin1/lab2/report/image/1.png){#fig:001 width=70%}

2) Провёл настройку маршрутизатора. Задали имя в виде "город-территория-учётная запись-номер".

![Имя маршрутизатора](/home/aalushin1/lab2/report/image/2.png){#fig:002 width=70%}

3) Задал интерфейсу FE с номером 0 ip адрес 192.168.1.254 и маску 255.255.255.0. Затем поднял интерфейс.

![Назначение ip адреса](/home/aalushin1/lab2/report/image/3.png){#fig:003 width=70%}

4) Проверил работоспособность соединение и с помощью пингов.

![Работоспособность соединения](/home/aalushin1/lab2/report/image/4.png){#fig:004 width=70%}

5) Задал пароль для доступа к привилегированному режиму (сначала в открытом видео, потом в зашифрованном)

![Установка пароля в открытом виде](/home/aalushin1/lab2/report/image/5.png){#fig:005 width=70%}

![Установка пароля в зашифрованном виде](/home/aalushin1/lab2/report/image/6.png){#fig:006 width=70%}

![Активация пароля](/home/aalushin1/lab2/report/image/7.png){#fig:007 width=70%}

6) Настроил доступ к оборудования через telnet. 

![Подключение через telnet](/home/aalushin1/lab2/report/image/8.png){#fig:008 width=70%}

7) Для пользователя admin задал доступ 1-го уровня по паролю.

![Пароль для админа](/home/aalushin1/lab2/report/image/9.png){#fig:009 width=70%}

8) Настроил доступ к оборудованию по ssh.

![Настройка ssh](/home/aalushin1/lab2/report/image/10.png){#fig:010 width=70%}

9) Подключился к оборудованию через ssh.

![Подключение по ssh](/home/aalushin1/lab2/report/image/11.png){#fig:011 width=70%}

10) Сохранили и экспортировали конфигурацию маршрутизатора в отдельном файле.

11) Провёл настройку коммутатора. Задал имя в виде "город-территория-учётная запись-номер".

![Имя для коммутатора](/home/aalushin1/lab2/report/image/12.png){#fig:012 width=70%}

12) Задал интерфейсу vlan 2 ip-адрес 192.168.2.1 и маску 255.255.255.0. Затем поднял интерфейс. 

![Адрес для коммутатора](/home/aalushin1/lab2/report/image/13.png){#fig:013 width=70%}

13) Привязал интерфейса FE с номером 1 к vlan2.

![Привязка FE к vlan2](/home/aalushin1/lab2/report/image/14.png){#fig:014 width=70%}

14) Задал в качестве адреса шлюза адрес 192.168.2.254

![Адрес шлюза](/home/aalushin1/lab2/report/image/15.png){#fig:015 width=70%}

15) Проверил работоспособность сети с помощью пингования.

![Проверка работоспособности](/home/aalushin1/lab2/report/image/16.png){#fig:016 width=70%}

16) Задал пароль для привилегированного режима (общий и зашифрованный)

![Выдача открытого пароля](/home/aalushin1/lab2/report/image/17.png){#fig:017 width=70%}

![Выдача зашифрованного пароля](/home/aalushin1/lab2/report/image/18.png){#fig:018 width=70%}

![Активация пароля](/home/aalushin1/lab2/report/image/19.png){#fig:019 width=70%}

17) Настроил подключение через telnet. 

![Подключение по telnet](/home/aalushin1/lab2/report/image/20.png){#fig:020 width=70%}

18) Для пользователя админ задал доступ 1-го уровня по паролю.

![Доступ для админа](/home/aalushin1/lab2/report/image/21.png){#fig:021 width=70%}

19) Настроил подключение по ssh и подключился. 

![Настройка ssh](/home/aalushin1/lab2/report/image/22.png){#fig:022 width=70%}

![Подключение по ssh](/home/aalushin1/lab2/report/image/23.png){#fig:023 width=70%}

# Выводы

Я получил основные навыки по начальному конфигурированию оборудования Cisco.



















