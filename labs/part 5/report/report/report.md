---
## Front matter
title: "Отчёт по реализации индивидуального проекта. Часть 5"
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

Добавить к сайту все остальные элементы. Сделать пост по прошедшей неделе. Добавить пост по тему "Языки научного программирования".

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

Перешёл в директорию с сайтом (рис. [-@fig:001]).

![Папка admin](image/1.PNG){#fig:001 width=70%}

Cобрал сайт (рис. [-@fig:002]).

![Сборка сайта](image/2.PNG){#fig:002 width=70%}

Запустил процесс для работы сайта (рис. [-@fig:003]).

![Запуск процесса для сайта](image/3.PNG){#fig:003 width=70%}

Перешёл в директорию content/project (рис. [-@fig:004]).

![Папка project](image/4.PNG){#fig:004 width=70%}

Переименновал директории (рис. [-@fig:005]).

![Переименнованные папки](image/5.PNG){#fig:005 width=70%}

Изменил файл index.md в директории Nitshe game (рис. [-@fig:006]).

![Измененённый файл index.md](image/6.PNG){#fig:006 width=70%}

Заменил картинку в директории Nitshe game (рис. [-@fig:007]).

![Заменённая картинка](image/7.PNG){#fig:007 width=70%}

Заменил картинку в директории Discord bot (рис. [-@fig:008]).

![Заменённая картинка](image/8.PNG){#fig:008 width=70%}

Изменил файл index.md в директории Nitshe game (рис. [-@fig:009]).

![Измененённый файл index.md](image/9.PNG){#fig:009 width=70%}

Открыл сайт и проверил список проектов (рис. [-@fig:010]).

![Проекты](image/10.PNG){#fig:010 width=70%}

Проверил проект Nitshe game (рис. [-@fig:011]).

![Проект](image/11.PNG){#fig:011 width=70%}

Проверил проект Discord bot (рис. [-@fig:012]).

![Проект](image/12.PNG){#fig:012 width=70%}

Перешёл в директорию content/post (рис. [-@fig:013]).

![Папка post](image/13.PNG){#fig:013 width=70%}

Скопировал директорию previous week 3 и переименновал её в previous week 4 (рис. [-@fig:014]).

![Смена имени для директории](image/14.PNG){#fig:014 width=70%}

Изменил файл index.md в директории previous week 4 (рис. [-@fig:015]).

![Измененённый файл index.md](image/15.PNG){#fig:015 width=70%}

Скопировал директорию Git и переименновал её в Scintific Programing languages (рис. [-@fig:018]).

![Смена имени для директории](image/18.PNG){#fig:018 width=70%}

Изменил файл index.md в директории Scintific Programing languages (рис. [-@fig:019], [-@fig:020], [-@fig:021]).

![Первая часть измененённого файла index.md](image/19.PNG){#fig:019 width=70%}

![Вторая часть измененённого файла index.md](image/20.PNG){#fig:020 width=70%}

![Третья часть измененённого файла index.md](image/21.PNG){#fig:021 width=70%}

Заменил картинку в директории Scintific Programing languages (рис. [-@fig:022]).

![Заменённая картинка](image/22.PNG){#fig:022 width=70%}

Открыл сайт и проверил список постов (рис. [-@fig:023]).

![Посты](image/0-1.PNG){#fig:023 width=70%}

Проверил пост за прошедшую неделю (4) (рис. [-@fig:024]).

![Часть поста](image/0-2.PNG){#fig:024 width=70%}

Проверил пост на тему языки научного программирования (рис. [-@fig:025]).

![Часть поста](image/0-3.PNG){#fig:025 width=70%}

# Выводы

Были приобретены навыки изменения блока проектов.

# Список литературы{.unnumbered}

::: {#refs}
:::
