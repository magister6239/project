---
## Front matter
title: "Отчёт по реализации индивидуального проекта. Часть 3"
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

Добавить к сайту достижения. Сделать пост по прошедшей неделе. Добавить пост.

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

Перешёл в папку с сайтом и собрал его (рис. [-@fig:001]).

![Сборка сайта](image/1.PNG){#fig:001 width=70%}

Запустил сайт (рис. [-@fig:002]).

![Запуск сайта](image/2.PNG){#fig:002 width=70%}

Перешёл в папку content/authors/admin и открыл файл _index.md (рис. [-@fig:003]).

![Открытие файла _index.md](image/3.PNG){#fig:003 width=70%}

Изменил элементы Technical и Hobbies в skills (рис. [-@fig:004], [-@fig:005]).

![Часть Technical](image/4.PNG){#fig:004 width=70%}

![Часть Hobbies](image/5.PNG){#fig:005 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:006]).

![Изменения](image/6.PNG){#fig:006 width=70%}

Перешёл в папку content и открыл файл _index.md (рис. [-@fig:100]).

![Открытие файла _index.md](image/7-0.PNG){#fig:100 width=70%}

Изменил блок Experience (рис. [-@fig:007]).

![Блок Experience](image/3-0.PNG){#fig:007 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:101]).

![Изменения](image/0-.PNG){#fig:101 width=70%}

Изменил блок Accomplishments(рис. [-@fig:102]).

![Блок Accomplishments](image/7.PNG){#fig:102 width=70%}

Переместил в папку assets/media/icons/brands (рис. [-@fig:103]).

![Иконки](image/-1.PNG){#fig:103 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:104]).

![Изменения](image/2-.PNG){#fig:104 width=70%}

Перешёл в папку content/post (рис. [-@fig:008]).

![Открытие файла _index.md](image/8.PNG){#fig:008 width=70%}

Создал папку для поста с именем markdown (рис. [-@fig:009]).

![Создание папки markdown](image/9.PNG){#fig:009 width=70%}

Скопировал файлы из поста про Git (рис. [-@fig:010]).

![Файлы](image/10.PNG){#fig:010 width=70%}

Заменил картинку для поста (рис. [-@fig:011]).

![Файлы](image/11.PNG){#fig:011 width=70%}

Прервал процесс отвечающий за работу сайта и пересобрал сайт (рис. [-@fig:012]).

![Прерванный процесс и повторный запуск](image/12.PNG){#fig:012 width=70%}

Запустил процесс для работы сайта (рис. [-@fig:013]).

![Запуск процесса для сайта](image/13.PNG){#fig:013 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:014]).

![Добавленный пост](image/14.PNG){#fig:014 width=70%}

Изменил файл index в папке content/post/markdown для поста (рис. [-@fig:015], [-@fig:016]).

![Начало поста](image/15.PNG){#fig:015 width=70%}

![Конец поста](image/16.PNG){#fig:016 width=70%}

Прервал процесс отвечающий за работу сайта и пересобрал сайт (рис. [-@fig:017]).

![Прерванный процесс и повторный запуск](image/17.PNG){#fig:017 width=70%}

Запустил процесс для работы сайта (рис. [-@fig:018]).

![Запуск процесса для сайта](image/18.PNG){#fig:018 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:019]).

![Изменённый пост](image/19.PNG){#fig:019 width=70%}

Открыл пост и проверил его (рис. [-@fig:020]).

![Часть поста](image/20.PNG){#fig:020 width=70%}

Перешёл в папку content/post и скопировал папку с постом за прошлую неделю (рис. [-@fig:021]).

![Открытие файла _index.md](image/21.PNG){#fig:021 width=70%}

Переименовал папку скопированну папку (рис. [-@fig:022]).

![Переименнование](image/22.PNG){#fig:022 width=70%}

Изменил файл index в папке content/post/previous week 2 для поста (рис. [-@fig:023]).

![Начало поста](image/23.PNG){#fig:023 width=70%}

Заменил картинку для поста (рис. [-@fig:024]).

![Файлы](image/24.PNG){#fig:024 width=70%}

Прервал процесс отвечающий за работу сайта и пересобрал сайт (рис. [-@fig:025]).

![Прерванный процесс и повторный запуск](image/25.PNG){#fig:025 width=70%}

Запустил процесс для работы сайта (рис. [-@fig:026]).

![Запуск процесса для сайта](image/26.PNG){#fig:026 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:027]).

![Добавленный пост](image/27.PNG){#fig:027 width=70%}

Открыл пост и проверил его (рис. [-@fig:028]).

![Часть поста](image/28.PNG){#fig:028 width=70%}

# Выводы

Были приобретены навыки изменения шаблона сайта и добавления новых элементов.

# Список литературы{.unnumbered}

::: {#refs}
:::
