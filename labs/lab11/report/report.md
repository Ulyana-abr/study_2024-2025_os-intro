---
## Front matter
title: "Отчет по лабораторной работе №11"
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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs.

# Задание

1. Ознакомиться с теоретическим материалом.
2. Ознакомиться с редактором emacs.
3. Выполнить упражнения.



# Выполнение лабораторной работы

Открываю emacs (рис. [-@fig:001]).

![emacs](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/1.jpg){#fig:001 width=70%}

Создаю файл lab07.sh с помощью комбинации Ctrl-x Ctrl-f и набираю необходимый текст (рис. [-@fig:002])

![изменение файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/2.jpg){#fig:002 width=70%}

Сохраняю файл с помощью комбинации Ctrl-x Ctrl-s.

Далее проделываю с текстом стандартные процедуры редактирования, осуществленное комбинацией клавиш.
Вырезаю командой "С-k" целую строку и вставляю ее в конец файла (C-y), после чего выделяю текст благодаря "C-space" 
(рис. [-@fig:003])

![изменение текста](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/3.jpg){#fig:003 width=70%}

Скопировав область в буфер обмена с помощью "M-w", вставляю область в конец файла. (рис. [-@fig:004])

![изменение текста](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/4.jpg){#fig:004 width=70%}

Вновь выделяю эту область и на этот раз вырезаю её, используя "C-w".
Отменяю последнее действие благодаря "C-/"

Далее учусь использовать команды по перемещению курсора:
- перемещение курсора в начало строки - "C-a"
- перемещение курсора в конец строки  - "C-e"
- перемещение курсора в начало буфера  - "M-<"
- перемещение курсора в конец буфера - "M->"

Вывожу список активных буферов на экран (C-x C-b).  (рис. [-@fig:005])

![вывод активных буферов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/5.jpg){#fig:005 width=70%}

Перемещаюсь во вновь открытое окно (C-x o) со списком открытых буферов и переключитесь на другой буфер. (рис. [-@fig:006])

![переключение на другой буфер](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/6.jpg){#fig:006 width=70%}

Закрываю это окно (C-x 0). (рис. [-@fig:007])

![закрытие окна](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/7.jpg){#fig:007 width=70%}

Теперь вновь переключаюсь между буферами, но уже без вывода их списка на экран (C-x b)

Разделяю фрейм на два окна по вертикали (C-x 3) (рис. [-@fig:008]) , а затем каждое из этих окон на две части по горизонтали (C-x 2) (рис. [-@fig:009])

![разделение фрейма](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/8.jpg){#fig:008 width=70%}

![разделение фрейма](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/9.jpg){#fig:009 width=70%}

В каждом из четырёх созданных окон открываю новый буфер (рис. [-@fig:010])

![открытие буфера](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/10.jpg){#fig:010 width=70%}

Переключаюсь в режим поиска (C-s) и нахожу несколько слов, присутствующих в тексте. (рис. [-@fig:011]) 

![режим поиска](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/11.jpg){#fig:011 width=70%}

Переключаюсь между результатами поиска, нажимая C-s. Выхожу из режима поиска, нажав C-g.
Перехожу в режим поиска и замены (M-%), ввожу текст, который следует найти и заменить, нажимаю Enter , затем ввожу текст для замены. После того как подсветились результаты поиска, нажимаю ! для подтверждения замены. (рис. [-@fig:012]) 

![режим поиска и замены](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab11/report/image/12.jpg){#fig:012 width=70%}

Испробую другой режим поиска, нажав M-s o, который отличается от обычного нахождением файла, а не фрагмента текста.

# Выводы

В данной работе мы познакомились с еще одним редактором операционной
системой Linux. Получили практические навыки работы с редактором Emacs.

# Список литературы{.unnumbered}

1. [Операционные системы](https://esystem.rudn.ru/pluginfile.php/2586728/mod_resource/content/5/009-lab_emacs.pdf)
