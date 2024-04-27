---
## Front matter
title: "Отчёт по реализации индивидуального проекта. Часть 4"
subtitle: "Дисциплина: Архитектура ЭВМ"
author: "Перегудов Александр Вадимович"

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
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

Приобрести навыки добавления на сайт дополнительных элементов.

# Задание

Добавить к сайту ссылки на научные и библиометрические ресурсы. Сделать пост по прошедшей неделе. Добавить пост по тему "Оформление отчёта".

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно про Unix см. в [@tanenbaum_book_modern-os_ru; @robbins_book_bash_en; @zarrelli_book_mastering-bash_en; @newham_book_learning-bash_en].

# Выполнение лабораторной работы

Перешёл в папку с сайтом а после в папку content/authors/admin (рис. [-@fig:001]).

![Папка admin](image/1.PNG){#fig:001 width=70%}

Открыл файл _index.md (рис. [-@fig:002]).

![Файл _index.md](image/2.PNG){#fig:002 width=70%}

Изменил элемент Social (рис. [-@fig:003]).

![Изменения](image/3.PNG){#fig:003 width=70%}

Пересобрал сайт (рис. [-@fig:100]).

![Сборка сайта](image/0-0.PNG){#fig:100 width=70%}

Запустил процесс для работы сайта (рис. [-@fig:101]).

![Запуск процесса для сайта](image/0-1.PNG){#fig:101 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:102]).

![Добавленные ссылки и иконки](image/0-2.PNG){#fig:102 width=70%}

Перешёл в папку content/post (рис. [-@fig:004]).

![Папка post ](image/4.PNG){#fig:004 width=70%}

Скопировал один из постов (рис. [-@fig:005]).

![Скопированный пост за прошлую неделю](image/5.PNG){#fig:005 width=70%}

Переименовал скопированную папку в previous week 3 (рис. [-@fig:006]).

![Переименнование](image/6.PNG){#fig:006 width=70%}

Изменил файл index в папке content/post/previous week 3 для поста (рис. [-@fig:07]).

![Файл index](image/7.PNG){#fig:07 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:008]).

![Добавленный пост](image/8.PNG){#fig:008 width=70%}

Открыл и проверил пост (рис. [-@fig:009]).

![Пост](image/9.PNG){#fig:009 width=70%}

Скопировал один из постов (рис. [-@fig:010]).

![Скопированный пост на тему markdown](image/10.PNG){#fig:010 width=70%}

Переименовал скопированную папку в report (рис. [-@fig:011]).

![Переименнование](image/11.PNG){#fig:011 width=70%}

Перешёл в папку report (рис. [-@fig:012]).

![Папка report](image/12.PNG){#fig:012 width=70%}

Заменил картинку для поста (рис. [-@fig:013]).

![Файлы](image/13.PNG){#fig:013 width=70%}

Изменил файл index в папке content/post/report для поста (рис. [-@fig:014], [-@fig:015], [-@fig:016], [-@fig:017]).

![Часть содержимого файла index](image/14.PNG){#fig:014 width=70%}

![Часть содержимого файла index](image/15.PNG){#fig:015 width=70%}

![Часть содержимого файла index](image/16.PNG){#fig:016 width=70%}

![Часть содержимого файла index](image/17.PNG){#fig:017 width=70%}

Пересобрал сайт (рис. [-@fig:018]).

![Сборка сайта](image/18.PNG){#fig:018 width=70%}

Запустил процесс для работы сайта (рис. [-@fig:019]).

![Запуск процесса для сайта](image/19.PNG){#fig:019 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:020]).

![Добавленный пост](image/20.PNG){#fig:020 width=70%}

Открыл и проверил пост (рис. [-@fig:021]).

![Часть поста](image/21.PNG){#fig:021 width=70%}

# Выводы

Были приобретены навыки изменения шаблона сайта и добавления новых элементов.

# Список литературы{.unnumbered}

::: {#refs}
:::
