---
## Front matter
title: "Отчет по лабораторной работе №9"
subtitle: "Дисциплина:Операционные системы"
author: "Абрамова Ульяна Михайловна"

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

Освоение основных возможностей командной оболочки Midnight Commander. Приобретение навыков практической работы по просмотру каталогов и файлов; манипуляций
с ними.

# Задание

1. Задание по mc
2. Задание по встроенному редактору mc

# Выполнение лабораторной работы
## Задание по mc
Изучаю информацию о mc, вызвав в командной строке man mc (рис. [-@fig:001]).

![man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/1.jpg){#fig:001 width=70%}

Выполняю несколько операций в mc, используя управляющие клавиши (рис. [-@fig:002], [-@fig:003], [-@fig:004])

![копирование файлов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2.jpg){#fig:002 width=70%}

![перемещение файлов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/3.jpg){#fig:003 width=70%}

![получение информации о размере и правах доступа на файлы](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/4.jpg){#fig:004 width=70%}

Выполняю основные команды меню правой панели (рис. [-@fig:004], [-@fig:005], [-@fig:006])

![![получение информации о размере и правах доступа на файлы](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/4.jpg){#fig:004 width=70%}

![быстрый просмотр](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/5.jpg){#fig:005 width=70%}

![дерево каталогов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/6.jpg){#fig:006 width=70%}

Используя возможности подменю Файл , выполняю различные команды (рис. [-@fig:007], [-@fig:008], [-@fig:009], [-@fig:010])

![просмотр содержимого текстового файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/7.jpg){#fig:007 width=70%}

![редактирование содержимого текстового файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/8.jpg){#fig:008 width=70%}

![создание каталога](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/9.jpg){#fig:009 width=70%}

![копирование в файлов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/10.jpg){#fig:010 width=70%}

С помощью соответствующих средств подменю Команда выполняю различные команды (рис. [-@fig:011], [-@fig:012], [-@fig:013], [-@fig:014])

![поиск в файловой системе файла с заданными условиями](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/11.jpg){#fig:011 width=70%}

![переход в домашних каталог](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/12.jpg){#fig:012 width=70%}

![анализ файла меню](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/13.jpg){#fig:013 width=70%}

![анализ файла расширений](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/14.jpg){#fig:014 width=70%}

Вызвав подменю Настройки, осваиваю операции, определяющие структуру экрана mc (рис. [-@fig:015], [-@fig:016], [-@fig:017], [-@fig:018], [-@fig:019], [-@fig:020], [-@fig:021], [-@fig:022])

![параметры конфигурации](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/15.jpg){#fig:015 width=70%}

![внешний вид](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/16.jpg){#fig:016 width=70%}

![настройки панели](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/17.jpg){#fig:017 width=70%}

![подтверждение](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/18.jpg){#fig:018 width=70%}

![оформление](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/19.jpg){#fig:019 width=70%}

![биты символов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/20.jpg){#fig:020 width=70%}

![определение клавиш](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/21.jpg){#fig:021 width=70%}

![настройки виртуальной файловой системы](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/22.jpg){#fig:022 width=70%}

## Задание по встроенному редактору mc
Создаю текстовой файл text.txt и откройте его с помощью редактора, затем вставляю в этот файл фрагмент текста, взятый из Интернета (рис. [-@fig:023])

![создание и изменение файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/23.jpg){#fig:023 width=70%}

С помощью горячей клавиши f8 удаляю строку, с помощью f5 копирую часть текста и вставляю на новую строчку (рис. [-@fig:024])

![изменение файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/24.jpg){#fig:024 width=70%}

С помощью f2 сохраняю файл, а благодаря ctrl+u отменяю последнее действие (рис. [-@fig:025])

![сохранение файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/25.jpg){#fig:025 width=70%}

С помощью ctrl+x перехожу в конец файла и добавляю текст (рис. [-@fig:026])

![изменение файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/26.jpg){#fig:026 width=70%}

С помощью ctrl+z перехожу в начало файла и добавляю текст (рис. [-@fig:027])

![изменение файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/27.jpg){#fig:027 width=70%}

Далее сохраняю и закрываю файл  (рис. [-@fig:028])

![выход из файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/28.jpg){#fig:028 width=70%}

# Выводы

В данной работе я ознакомилась с инструментами командной оболочки Midnight Commander. Приобрела навыки практической работы по просмотру каталогов и файлов

# Список литературы{.unnumbered}

1. [Операционные системы](https://esystem.rudn.ru/pluginfile.php/2586724/mod_resource/content/5/007-lab_mc.pdf)
