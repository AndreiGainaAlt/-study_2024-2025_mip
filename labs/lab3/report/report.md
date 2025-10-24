---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: "Моделирование стохастических процессов"
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

Провести моделирование системы массового обслуживания (СМО).

# Задание

1. Реализовать модель М|М|1.
2. Посчитать загрузку системы и вероятность потери пакетов.
3. Построить график изменения размера очереди.

# Выполнение лабораторной работы

Реализовал модель М|М|1 на NS-2 (рис. [-@fig:001])

![Реализация модели на NS-2](image/1.png){ #fig:001 width=70% }

Запустил программу. Получил данные о теор. вероятности потери, теор. средней длины очереди (рис. [-@fig:002])

![Запуск программы](image/2.png){ #fig:002 width=70% }

Создал файл graph_plot (рис. [-@fig:003])

![Создание файла graph_plot](image/4.png){ #fig:003 width=70% }

Создал исполняемый файл graph_plot и запустил его (рис. [-@fig:005])

![Исполняемый файл graph_plot](image/5.png){ #fig:005 width=70% }

Программа создала файл qm.pdf с графиком поведения длины очереди (рис. [-@fig:006])

![График поведения длины очереди](image/6.png){ #fig:006 width=70% }

# Выводы

Провел моделирование системы массового обслуживания (СМО).