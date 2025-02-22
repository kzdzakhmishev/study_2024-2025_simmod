---
## Front matter
title: "Отчёт по лабораторной работе"
subtitle: "Лабораторная №3 по имитационному моделированию"
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

Требуется разработать сценарий, реализующий модель согласно рис. 2.4, построить в Xgraph график изменения TCP-окна, график изменения длины очереди и средней длины очереди



# Выполнение лабораторной работы

![Создание модели по приведённому коду.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab03/1/1.png){#fig:001 width=70%}

# Выполнение лабораторной работы

![Создание модели по приведённому коду.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab03/1/2.png){#fig:002 width=70%}

# Выполнение лабораторной работы

![Создание модели по приведённому коду.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab03/1/3.png){#fig:003 width=70%}

# Выполнение лабораторной работы

![Теор. вероятность потери и средняя длина очереди](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab03/1/4.png){#fig:004 width=70%}

# Выполнение лабораторной работы

![Список](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab03/1/5.png){#fig:005 width=70%}

# Выполнение лабораторной работы

![graph_plot](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab03/1/6.png){#fig:006 width=70%}

# Выполнение лабораторной работы

![Файл qm появился](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab03/1/7.png){#fig:007 width=70%}

# Выполнение лабораторной работы

![Содержимое графика qm](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab03/1/8.png){#fig:008 width=70%}


# Выводы

В ходе данной лабораторной работы составил график задачи по вычислению средней длины очереди.

# Список литературы{.unnumbered}

::: {#refs}
:::
