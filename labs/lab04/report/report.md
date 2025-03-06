---
## Front matter
title: "Отчёт по лабораторной работе"
subtitle: "Выполнение задания по имитационному моделированию"
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

Построить с помощью xcos фигуры Лиссажу с различными значениями параметров.

# Задание

Постройте с помощью xcos фигуры Лиссажу со следующими параметрами:
1) A = B = 1, a = 2, b = 2, δ = 0; π/4; π/2; 3π/4; π;
2) A = B = 1, a = 2, b = 4, δ = 0; π/4; π/2; 3π/4; π;
3) A = B = 1, a = 2, b = 6, δ = 0; π/4; π/2; 3π/4; π;
4) A = B = 1, a = 2, b = 3, δ = 0; π/4; π/2; 3π/4; π.

# Выполнение лабораторной работы

![Строение нашей модели.](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/1.png){#fig:001 width=70%}

# Выполнение лабораторной работы

![Ввод значений для первого блока с частотой 2 и значением фазы 0](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/2.png){#fig:002 width=70%}

# Выполнение лабораторной работы

![Ввод значений для второго блока с частотой 2](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/3.png){#fig:003 width=70%}

# Выполнение лабораторной работы

![График с первым значением фазы (дельта = 0)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/4.png){#fig:004 width=70%}

# Выполнение лабораторной работы

![Ввод значений для первого блока со значением фазы pi/4](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/5.png){#fig:005 width=70%}

# Выполнение лабораторной работы

![График со вторым значением фазы (дельта =  pi/4)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/6.png){#fig:006 width=70%}

# Выполнение лабораторной работы

![Ввод значений для первого блока со значением фазы pi/2](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/7.png){#fig:007 width=70%}

# Выполнение лабораторной работы

![График с третьим значением фазы (дельта =  pi/2)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/8.png){#fig:008 width=70%}

# Выполнение лабораторной работы

![Ввод значений для первого блока со значением фазы 3pi/4](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/9.png){#fig:009 width=70%}

# Выполнение лабораторной работы

![График с четвертым значением фазы (дельта =  3pi/4)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/10.png){#fig:010 width=70%}

# Выполнение лабораторной работы

![Ввод значений для первого блока со значением фазы pi](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/11.png){#fig:011 width=70%}

# Выполнение лабораторной работы

![График с пятым значением фазы (дельта =  pi)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/12.png){#fig:012 width=70%}

# Выполнение лабораторной работы

![Ввод значений для второго блока с частотой 4 и значением фазы 0](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/13.png){#fig:013 width=70%}

# Выполнение лабораторной работы

![График с первым значением фазы (дельта =  0)](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/14.png){#fig:014 width=70%}

# Выполнение лабораторной работы

![График со значением фазы pi/4](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/15.png){#fig:015 width=70%}

# Выполнение лабораторной работы

![pi/2](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/16.png){#fig:016 width=70%}

# Выполнение лабораторной работы

![3pi/4](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/17.png){#fig:017 width=70%}

# Выполнение лабораторной работы

![pi](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/18.png){#fig:018 width=70%}

# Выполнение лабораторной работы

![Значение частоты = 6](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/19.png){#fig:019 width=70%}

# Выполнение лабораторной работы

![Дельта = 0](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/20.png){#fig:020 width=70%}

# Выполнение лабораторной работы

![Дельта = pi/4](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/21.png){#fig:021 width=70%}

# Выполнение лабораторной работы

![Дельта = pi/2](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/22.png){#fig:022 width=70%}

# Выполнение лабораторной работы

![Дельта = 3pi/4](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/23.png){#fig:023 width=70%}

# Выполнение лабораторной работы

![Частота = 3](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/24.png){#fig:024 width=70%}

# Выполнение лабораторной работы

![Дельта = 0](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/25.png){#fig:025 width=70%}

# Выполнение лабораторной работы

![Дельта = pi/4](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/26.png){#fig:026 width=70%}

# Выполнение лабораторной работы

![Дельта = pi/2](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/27.png){#fig:027 width=70%}

# Выполнение лабораторной работы

![Дельта = 3pi/4](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/28.png){#fig:028 width=70%}

# Выполнение лабораторной работы

![Дельта = pi](/home/kambulat/work/study/2024-2025/Имитационное моделирование/study_2024-2025_simmod/labs/lab04/1/29.png){#fig:029 width=70%}

# Выводы

В ходе данной работы Я научился строить с помощью xcos фигуры Лиссажу с различными значениями параметров.

# Список литературы{.unnumbered}

::: {#refs}
:::
