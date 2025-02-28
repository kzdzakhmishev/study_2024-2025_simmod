---
## Front matter
title: "Отчёт по лабораторной работе"
subtitle: "Лабораторная №4 по имитационному моделированию"
author: "Дзахмишев Камбулат Заурович"

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
lot: true # List of tables
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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Описание моделируемой сети:
– сеть состоит из 6 узлов;
– между всеми узлами установлено дуплексное соединение с различными пропуск-
ной способностью и задержкой 10 мс (см. рис. 2.4);
– узел r1 использует очередь с дисциплиной RED для накопления пакетов, макси-
мальный размер которой составляет 25;
– TCP-источники на узлах s1 и s2 подключаются к TCP-приёмнику на узле s3;
– генераторы трафика FTP прикреплены к TCP-агентам.

# Задание

Т– сеть состоит из N TCP-источников, N TCP-приёмников, двух маршрутизаторов
R1 и R2 между источниками и приёмниками (N — не менее 20);
– между TCP-источниками и первым маршрутизатором установлены дуплексные
соединения с пропускной способностью 100 Мбит/с и задержкой 20 мс очередью
типа DropTail;
– между TCP-приёмниками и вторым маршрутизатором установлены дуплексные
соединения с пропускной способностью 100 Мбит/с и задержкой 20 мс очередью
типа DropTail;

# Задание

– между маршрутизаторами установлено симплексное соединение (R1–R2) с про-
пускной способностью 20 Мбит/с и задержкой 15 мс очередью типа RED,
размером буфера 300 пакетов; в обратную сторону — симплексное соедине-
ние (R2–R1) с пропускной способностью 15 Мбит/с и задержкой 20 мс очередью
типа DropTail;
– данные передаются по протоколу FTP поверх TCPReno;
– параметры алгоритма RED: qmin = 75, qmax = 150, qw = 0, 002, pmax = 0.1;
– максимальный размер TCP-окна 32; размер передаваемого пакета 500 байт; время
моделирования — не менее 20 единиц модельного времени.

# Задание

1. Для приведённой схемы разработать имитационную модель в пакете NS-2.
2. Построить график изменения размера окна TCP (в Xgraph и в GNUPlot);
3. Построить график изменения длины очереди и средней длины очереди на первом
маршрутизаторе.
4. Оформить отчёт о выполненной работе.

# Выполнение лабораторной работы

![Модель из самостоятельного задания.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/1.png){#fig:001 width=70%}

# Выполнение лабораторной работы

![Модель из самостоятельного задания.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/2.png){#fig:002 width=70%}

# Выполнение лабораторной работы

![Модель из самостоятельного задания.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/3.png){#fig:003 width=70%}

# Выполнение лабораторной работы

![Модель из самостоятельного задания.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/4.png){#fig:004 width=70%}

# Выполнение лабораторной работы

![Изменение размера окна TCP на всех источниках при N=30](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/5.png){#fig:005 width=70%}

# Выполнение лабораторной работы

![Изменение размера окна TCP на линке 1-го источника при N=30](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/6.png){#fig:006 width=70%}

# Выполнение лабораторной работы

![Изменение размера средней длины очереди на линке (R1–R2)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/7.png){#fig:007 width=70%}

# Выполнение лабораторной работы

![Изменение размера длины очереди на линке (R1–R2)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/8.png){#fig:008 width=70%}

# Выполнение лабораторной работы

![Изменение размера окна TCP на всех источниках при N=30](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/9.png){#fig:009 width=70%}

# Выполнение лабораторной работы

![Изменение размера средней длины очереди на линке (R1–R2)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/10.png){#fig:010 width=70%}

# Выполнение лабораторной работы

![Текущая длина очереди на линке (R1–R2)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/11.png){#fig:011 width=70%}

# Выполнение лабораторной работы

![Изменение размера окна TCP на всех источниках при N=30](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/12.png){#fig:012 width=70%}


# Выводы

В ходе данной лабораторной работы Я:
Для приведённой схемы разработал имитационную модель в пакете NS-2.
Построил график изменения размера окна TCP (в Xgraph и в GNUPlot);
Построил график изменения длины очереди и средней длины очереди на первом
маршрутизаторе.

# Список литературы{.unnumbered}

::: {#refs}
:::
