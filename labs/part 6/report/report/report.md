---
## Front matter
title: "Отчёт по реализации индивидуального проекта. Часть 6"
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

Приобрести навыки настройки нескольких языков на примере конструктора Hugo.

# Задание

Сделать поддержку английского и русского языков.

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

Перешёл в корневую папку с сайтом и создал директорию i18n (рис. [-@fig:001]).

![Папка i18n](image/1.PNG){#fig:001 width=70%}

Скачал языковые файлы для русского и английского языков и скопировал их в директорию i18n (рис. [-@fig:002]).

![Языковые файлы в папке i18n](image/2.PNG){#fig:002 width=70%}

Перешёл в директорию _default, скопировал файл menus.yaml и переименновал его в menus.ru.yaml (рис. [-@fig:003]).

![Файл menus.ru.yaml](image/3.PNG){#fig:003 width=70%}

Изменил файл menus.ru.yaml (рис. [-@fig:004]).

![Перевод меню](image/4.PNG){#fig:004 width=70%}

В той же директории изменил файл languages.yaml (рис. [-@fig:005]).

![Добавил русский язык и указал папку с контентом для этого языка](image/5.PNG){#fig:005 width=70%}

Перешёл в директорию content, создал ru и en директории и скопировал все файлы и директории в content в эти дирекотрии (рис. [-@fig:006]).

![Директории en и ru](image/6.PNG){#fig:006 width=70%}

Перешёл в директорию en/post/previous week 4 (рис. [-@fig:007]).

![Пост previous week 4](image/7.PNG){#fig:007 width=70%}

Изменил файл index.md для английской версии сайта (рис. [-@fig:008]).

![Файл index.md](image/8.PNG){#fig:008 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:009]).

![Пост на английском языке](image/9.PNG){#fig:009 width=70%}

Перешёл в директорию en/post/Scintific Programming languages (рис. [-@fig:010]).

![Пост Programming languages](image/10.PNG){#fig:010 width=70%}

Изменил файл index.md для английской версии сайта (рис. [-@fig:100], [-@fig:101], [-@fig:102]).

![Часть содержимого файла index.md](image/0-0.PNG){#fig:100 width=70%}

![Часть содержимого файла index.md](image/0-1.PNG){#fig:101 width=70%}

![Часть содержимого файла index.md](image/0-2.PNG){#fig:102 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:011]).

![Пост на английском языке](image/11.PNG){#fig:011 width=70%}

После я изменил все посты, публикации и события. Процесс аналогичен двум выше а постов много. Для примера я описал изменения двух постов, но на самом деле изменил все. Для русской версии сайта тоже самое.

Перешёл в директорию en/ (рис. [-@fig:103]).

![Директория en/](image/0-3.PNG){#fig:103 width=70%}

Открыл и изменил файл _index.md (рис. [-@fig:012], [-@fig:013], [-@fig:014], [-@fig:015], [-@fig:016], [-@fig:017], [-@fig:018], [-@fig:019]).

![Часть содержимого файла _index.md](image/12.PNG){#fig:012 width=70%}

![Часть содержимого файла _index.md](image/13.PNG){#fig:013 width=70%}

![Часть содержимого файла _index.md](image/14.PNG){#fig:014 width=70%}

![Часть содержимого файла _index.md](image/15.PNG){#fig:015 width=70%}

![Часть содержимого файла _index.md](image/16.PNG){#fig:016 width=70%}

![Часть содержимого файла _index.md](image/17.PNG){#fig:017 width=70%}

![Часть содержимого файла _index.md](image/18.PNG){#fig:018 width=70%}

![Часть содержимого файла _index.md](image/19.PNG){#fig:019 width=70%}

Тоже самое я сделал и для русской версии сайта. Процесс анологичен этому. Русская версия сайта находится в директории content/ru.

Пересобрал сайт и Запустил процесс для работы сайта (рис. [-@fig:020], [-@fig:021]).

![Команда для сборки сайта](image/20.PNG){#fig:020 width=70%}

![Команда для сборки сайта](image/21.PNG){#fig:021 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:022], [-@fig:023]).

![Сайт на английском языке](image/22.PNG){#fig:022 width=70%}

![Сайт на русском языке](image/23.PNG){#fig:023 width=70%}

Перешёл в директорию content/ru/post (рис. [-@fig:024]).

![Директория post](image/24.PNG){#fig:024 width=70%}

Скопировал директорию previous week 4 и переименновал её в previous week 5 (рис. [-@fig:025]).

![Директория previous week 5](image/25.PNG){#fig:025 width=70%}

Изменил файл index.md в директории previous week 5 (рис. [-@fig:026]).

![Измененённый файл index.md](image/26.PNG){#fig:026 width=70%}

В той же директории скопировал дирекотрию Git и переименновал её в Software architecture. (рис. [-@fig:027]).

![Директория Software architecture](image/27.PNG){#fig:027 width=70%}

Перешёл в директорию Software architecture и заменил картинку. (рис. [-@fig:028]).

![Новая картинка](image/28.PNG){#fig:028 width=70%}

Открыл и изменил файл index.md (рис. [-@fig:029]).

![Часть создержимого файла index.md](image/29.PNG){#fig:029 width=70%}

Скопировал директорию Software architecture в директорию content/en/post (рис. [-@fig:030]).

![Директория Software architecture](image/30.PNG){#fig:030 width=70%}

Открыл и изменил файл index.md (рис. [-@fig:031]).

![Часть создержимого файла index.md](image/31.PNG){#fig:031 width=70%}

Открыл сайт и проверил изменения (рис. [-@fig:032], [-@fig:033]).

![Часть поста на русском языке](image/32.PNG){#fig:032 width=70%}

![Часть поста на английском языке](image/33.PNG){#fig:033 width=70%}

# Выводы

Были приобретены навыки настройки языков на сайте.

# Список литературы{.unnumbered}

::: {#refs}
:::
