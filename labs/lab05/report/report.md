---
## Front matter
title: "Отчёт по лабораторной работе"
subtitle: "Лабораторная №5 по имитационному моделированию"
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

Реализуйте модель SIR в OpenModelica.

# Задание

Требуется разработать сценарий, реализующий модель согласно рис. 2.4, построить в Xgraph график изменения TCP-окна, график изменения длины очереди и средней длины очереди

# Задание

В дополнение к предположениям, которые были сделаны для модели SIR (5.1) , пред-
положим, что учитываются демографические процессы, в частности, что смертность
в популяции полностью уравновешивает рождаемость, а все рожденные индивидуу-
мы появляются на свет абсолютно здоровыми. Тогда получим следующую систему
уравнений:



˙s = −βs(t)i(t) + μ(N − s(t));
˙i = βs(t)i(t) − νi(t) − μi(t);
˙r = νi(t) − μr(t),

# Задание

где μ — константа, которая равна коэффициенту смертности и рождаемости.
Требуется:
– реализовать модель SIR с учётом процесса рождения / гибели особей в xcos (в
том числе и с использованием блока Modelica), а также в OpenModelica;
– построить графики эпидемического порога при различных значениях параметров
модели (в частности изменяя параметр μ);
– сделать анализ полученных графиков в зависимости от выбранных значений
параметров модели.

# Выполнение лабораторной работы

![Установка контекста и создание блочной модели](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/1.png){#fig:001 width=70%}

# Выполнение лабораторной работы

![Ввод значений начального состояния верхнего интеграла](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/2.png){#fig:002 width=70%}

# Выполнение лабораторной работы

![Ввод значений начального состояния нижнего интеграла](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/3.png){#fig:003 width=70%}

# Выполнение лабораторной работы

![Установка конечного времени интегрирования](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/4.png){#fig:004 width=70%}

В нашем случае оно равно 30.

# Выполнение лабораторной работы

![График модели эпидемии в xcos](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/5.png){#fig:005 width=70%}

# Выполнение лабораторной работы

![Реализация модели с помощью блока Modelica в xcos](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/6.png){#fig:006 width=70%}

В процессе установки параметров блока Моделика Я забыл сделать скриншот с вводом значений для него, к сожалению. График выходит тем же, что и раньше.

# Выполнение лабораторной работы

![Код для нашей SIR в OpenModelica](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/7.png){#fig:007 width=70%}

Также установил здесь время конечное равное 30 единицам. На выводе графика имеем тот же график, что и в предыдущих пунктах, только в OprnModelica.

# Выполнение лабораторной работы

![Модель для самостоятельного задания в OpenModelica](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/8.png){#fig:008 width=70%}

# Выполнение лабораторной работы

![График модели эпидемии](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/9.png){#fig:009 width=70%}

# Выполнение лабораторной работы

![График модели эпидемии и её модель в xcos](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/10.png){#fig:010 width=70%}

Уже здесь изменять начал устанавливать другой контекст, изменяя параметр mu.

# Выполнение лабораторной работы

![График модели эпидемии с изменёнными параметрами](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/11.png){#fig:011 width=70%}

# Выполнение лабораторной работы

![Изменение контекста к предыдущему графику](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab05/1/12.png){#fig:012 width=70%}

Здесь можно заметить, что число здоровых людей резко идет на спад, что влечёт по логиче за собой и резкое увеличение числа зараженных.

# Выводы

В ходе данной лабораторной работы составил графики и модели эпидемии, а также научился изменять параметры модели с целью ознакомления с ходом развития эпидемии.

# Список литературы{.unnumbered}

::: {#refs}
:::
