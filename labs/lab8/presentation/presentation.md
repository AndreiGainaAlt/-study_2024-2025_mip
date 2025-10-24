---
## Front matter
lang: ru-RU
title: Лабораторная Работа №8
subtitle: Модель TCP/AQM
author:
  - Гэинэ Андрей
institute:
  - Российский университет дружбы народов им. Патриса Лумумбы, Москва, Россия

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\makeatother'

## Fonts
mainfont: Arial
romanfont: Arial
sansfont: Arial
monofont: Arial
---


## Докладчик


  * Гэинэ Андрей
  * НФИбд-02-22
  * Российский университет дружбы народов
  * [1032219249@pfur.ru]
  
# Выполнение лабораторной работы

## Цель работы

Реализовать модель TCP/AQM в xcos и OpenModelica.

## Задание

1. Построить модель TCP/AQM в xcos;
2. Построить графики динамики изменения размера TCP окна W(t) и размера очереди Q(t);
3. Построить модель TCP/AQM в OpenModelica;

## Установил контекст

![Установка контекста](image/1.png){ #fig:001 width=70% }

## Реализовал модель TCP/AQM в xcod

![Реализация модели в xcos](image/2.png){ #fig:002 width=70% }

## Получил график динамики изменения размера TCP окна W(t) и размера очереди Q(t)

![Динамика изменения размера TCP окна W(t) и размера очереди Q(t)](image/3.png){ #fig:003 width=70% }

## Получил график фазового портрета (W, Q)

![Фазовый портрет (W, Q)](image/4.png){ #fig:004 width=70% }

## Написал код для реалищации модели в OpenModelica

![Код для OpenModelica](image/5.png){ #fig:005 width=70% }

## Получил график динамики изменения размера TCP окна W(t) и размера очереди Q(t)

![Динамика изменения размера TCP окна W(t) и размера очереди Q(t)](image/6.png){ #fig:006 width=70% }

## Получил график фазового портрета (W, Q)

![Фазовый портрет (W, Q)](image/7.png){ #fig:007 width=70% }

## Выводы

Реализовал модель TCP/AQM в xcos и OpenModelica.