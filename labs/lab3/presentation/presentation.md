---
## Front matter
lang: ru-RU
title: Лабораторная Работа №3
subtitle: Моделирование стохастических процессов
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

## Цель работы

Исследовать протокол TCP и алгоритм управления очередью RED.

## Задание

1. Реализовать модель М|М|1.
2. Посчитать загрузку системы и вероятность потери пакетов.
3. Построить график изменения размера очереди.

# Выполнение лабораторной работы

## Реализовал модель М|М|1 на NS-2

![Реализация модели на NS-2](image/1.png){ #fig:001 width=70% }

## Запустил программу. Получил данные о теор. вероятности потери, теор. средней длины очереди

![Запуск программы](image/2.png){ #fig:002 width=70% }

## Создал файл graph_plot

![Редактирование файла graph_plot](image/4.png){ #fig:004 width=70% }

## Создал исполняемый файл graph_plot и запустил его

![Исполняемый файл graph_plot](image/5.png){ #fig:005 width=70% }

## Программа создала файл qm.pdf с графиком поведения длины очереди

![График поведения длины очереди](image/6.png){ #fig:006 width=70% }

## Выводы

Провел моделирование системы массового обслуживания (СМО).