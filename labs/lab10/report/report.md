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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Задание

1. Создание нового файла с использованием vi
2. Редактирование существующего файла

# Выполнение лабораторной работы
## Создание нового файла с использованием vi
Создаю каталог с именем ~/work/os/lab06 и перейдите в него. Затем вызываю vi и создаю файл hello.sh. После чего нажимаю на клавишу "i" и ввожу текст (рис. [-@fig:001]).

![ввод текста](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/1.jpg){#fig:001 width=70%}

После завершения ввода текста нажимаю клавишу Esc для перехода в командный режим, далее нажимаю ":" для перехода в режим последней строки и нажимаю wq+enter, чтобы записать изменения и выйти (рис. [-@fig:002]).

![запись изменения и выход](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2.jpg){#fig:002 width=70%}

Делаю файл исполняемым (рис. [-@fig:003]).

![chmod](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/3.jpg){#fig:003 width=70%}

##Редактирование существующего файла
Вызываю vi на редактирование ранее созданного файла и вношу изменения в текст: 
1) в режиме вставки заменяю HELL во второй строке на HELLO, вместо LOCAL в четвертой строке набираю local, 
2) установив курсор на последней строке файла с помощью команды G, вставьте после неё строку с текстом: echo $HELLO.
Нажимаю на Esc для перехода в командный режим и удаляю эту строчку командой nd, где n - номер строки (рис. [-@fig:004]).

![изменения текста](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/4.jpg){#fig:004 width=70%}

3) ввожу команду отмены изменений u для отмены последней команды (рис. [-@fig:005]).

![отмена последней команды](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/5.jpg){#fig:005 width=70%}

Затем ввожу символ : для перехода в режим последней строки и благодаря wq+enter записываю изменения и выхожу из файла

# Выводы

В данной работе я познакомилась с операционной системой Linux и получила практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Список литературы{.unnumbered}

1. [Операционные системы](https://esystem.rudn.ru/pluginfile.php/2586726/mod_resource/content/4/008-lab_vi.pdf)
