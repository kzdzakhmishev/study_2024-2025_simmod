---
## Front matter
title: "Отчёт по лабораторной работе"
subtitle: "Лабораторная №7 по имитационному моделированию"
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

Реализовать модель М|М|1|inf в xcos.

# Выполнение лабораторной работы

![Установка контекста.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab07/1/1.png){#fig:001 width=70%}

# Выполнение лабораторной работы

![Суперблок, моделирующий поступление заявок.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab07/1/2.png){#fig:002 width=70%}

# Выполнение лабораторной работы

![Ввод функции.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab07/1/3.png){#fig:003 width=70%}

# Выполнение лабораторной работы

![Суперблок, моделирующий обработку заявок.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab07/1/4.png){#fig:004 width=70%}

# Выполнение лабораторной работы

![Сама модель M|M|inf в xcos.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab07/1/5.png){#fig:005 width=70%}

# Выполнение лабораторной работы

![Параметры моделировния (ставлю то же, что и в других лабах).](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab07/1/6.png){#fig:006 width=70%}

# Выполнение лабораторной работы

![График поступления (чёрный) и обработки (зелёный) заявок.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab07/1/7.png){#fig:007 width=70%}

# Выполнение лабораторной работы

![График динамики размера очереди.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab07/1/8.png){#fig:008 width=70%}

# Вывод

В ходе данной лабораторной работы построил модель М|М|1|inf и вывел графики поступления и обработки заявок, а также график динамики размера очереди в xcos.

# Список литературы{.unnumbered}

::: {#refs}
:::
