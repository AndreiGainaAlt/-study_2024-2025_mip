---
## Front matter
title: "Отчёт по лабораторной работе №2"
subtitle: "Исследование протокола TCP и алгоритма управления очередью RED"
author: "Гэинэ Андрей НФИбд-02-22"

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
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: Arial
romanfont: Arial
sansfont: Arial
monofont: Arial
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

Исследовать протокол TCP и алгоритм управления очередью RED.

# Задание

1. Выполнить пример с дисциплиной RED.
2. Изменить протокол TCP с Reno на NewReno, Vegas. Пояснить результаты.
3. Внести изменения в отображаемые графики.

# Выполнение лабораторной работы

Разработал сценарий, реализующий модель согласно рис. 2.4, построил в Xgraph график изменения TCP-окна, график изменения длины очереди
и средней длины очереди. (рис. [-@fig:001])

![График изменения TCP-окна, график изменения длины очереди](image/1.png){ #fig:001 width=70% }

Отобразил графики, запустив программу. Средняя длина очереди находится в диапазоне от 2 до 4. Макс. длина достигает значения 14. (рис. [-@fig:002])

![Отображение графиков для Reno](image/2.png){ #fig:002 width=70% }

Изменил тип с Reno на NewReno (рис. [-@fig:003])

![Изменение протокола TCP](image/3.png){ #fig:003 width=70% }

Отобразил графики, запустив программу. Значения длины очереди, макс. длины совпадает с предыдущими значениями. В обоих случаях окна увеличиваются до тех пор, пока не произойдет потеря сегмента (рис. [-@fig:004])

![Отображение графиков для NewReno 1](image/4.png){ #fig:004 width=70% }

![Отображение графиков для NewReno 2](image/4_1.png){ #fig:004 width=70% }

Изменил тип с Reno на Vegas (рис. [-@fig:005])

![Изменение протокола TCP](image/5.png){ #fig:005 width=70% }

Отобразил графики, запустив программу. Видно, что при Vegas макс. размер окна составляет 20, а не 34. TCP Vegas обнаруживает перегрузку до того, как теряется пакет, мгновенно уменьшается размер окна. (рис. [-@fig:006])

![Отображение графиков для Vegas 1](image/6.png){ #fig:006 width=70% }

![Отображение графиков для Vegas 2](image/6_1.png){ #fig:006 width=70% }

Внес изменения в код программы. Поменял цвет фона, траекторий , подписей. (рис. [-@fig:007])

![Изменение графиков](image/7.png){ #fig:007 width=70% }

Отобразил новые графики, запустив программу. (рис. [-@fig:008])

![Видоизмененные графики](image/8.png){ #fig:008 width=70% }

# Выводы

Исследовал протокол TCP и алгоритм управления очередью RED.