---
## Front matter
title: "Отчёт по лабораторной работе №8"
subtitle: "Модель TCP/AQM"
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

Реализовать модель TCP/AQM в xcos и OpenModelica.

# Задание

1. Построить модель TCP/AQM в xcos;
2. Построить графики динамики изменения размера TCP окна W(t) и размера очереди Q(t);
3. Построить модель TCP/AQM в OpenModelica;

# Выполнение лабораторной работы

Установил контекст (рис. [-@fig:001])

![Установка контекста](image/1.png){ #fig:001 width=70% }

Реализовал модель TCP/AQM в xcos (рис. [-@fig:002])

![Реализация модели в xcos](image/2.png){ #fig:002 width=70% }

Получил график динамики изменения размера TCP окна W(t) и размера очереди Q(t) (рис. [-@fig:003])

![Динамика изменения размера TCP окна W(t) и размера очереди Q(t)](image/3.png){ #fig:003 width=70% }

Получил график фазового портрета (W, Q) (рис. [-@fig:004])

![Фазовый портрет (W, Q)](image/4.png){ #fig:004 width=70% }

Написал код для реалищации модели в OpenModelica (рис. [-@fig:005])

![Код для OpenModelica](image/5.png){ #fig:005 width=70% }

Получил график динамики изменения размера TCP окна W(t) и размера очереди Q(t) (рис. [-@fig:006])

![Динамика изменения размера TCP окна W(t) и размера очереди Q(t)](image/6.png){ #fig:006 width=70% }

Получил график фазового портрета (W, Q) (рис. [-@fig:007])

![Фазовый портрет (W, Q)](image/7.png){ #fig:007 width=70% }

# Выводы

Реализовал модель TCP/AQM в xcos и OpenModelica.