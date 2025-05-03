---
## Front matter
title: "Отчет по лабораторной работе №12"
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

* Изучить основы программирования в оболочке ОС UNIX/Linux. 
* Научиться писать небольшие командные файлы.

# Задание

1. Написать скрипт, который при запуске будет делать резервную копию самого себя (то
есть файла, в котором содержится его исходный код) в другую директорию backup
в вашем домашнем каталоге. При этом файл должен архивироваться одним из архиваторов на выбор zip, bzip2 или tar. Способ использования команд архивации
необходимо узнать, изучив справку.
2. Написать пример командного файла, обрабатывающего любое произвольное число
аргументов командной строки, в том числе превышающее десять. Например, скрипт
может последовательно распечатывать значения всех переданных аргументов.
3. Написать командный файл — аналог команды ls (без использования самой этой команды и команды dir). Требуется, чтобы он выдавал информацию о нужном каталоге
и выводил информацию о возможностях доступа к файлам этого каталога.
4. Написать командный файл, который получает в качестве аргумента командной строки
формат файла (.txt, .doc, .jpg, .pdf и т.д.) и вычисляет количество таких файлов
в указанной директории. Путь к директории также передаётся в виде аргумента командной строки.



# Выполнение лабораторной работы
1. Написали скрипт, который при запуске делает резервную копию самого себя (то есть файла, в котором содержится его исходный код) в другую директорию backup в моём домашнем каталоге. При этом файл архивируется одним из архиваторов на выбор zip , bzip2 или tar . Способ использования команд архивации узнали, изучив справку. (рис. [-@fig:001], [-@fig:002]).
```
командой cp копируем файл в директорию ~/backup/, а командой gzip исходный файл архивируется и удаляется (остаётся только архив)
```

![1](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab12/report/image/1.jpg){#fig:001 width=70%}

![2](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab12/report/image/2.jpg){#fig:002 width=70%}

2. Написали пример командного файла, обрабатывающего любое произвольное число аргументов командной строки, в том числе превышающее десять. Например, скрипт может последовательно распечатывать значения всех переданных аргументов (рис. [-@fig:003], [-@fig:004]).

```
for i — для всех переданных аргументов
    do echo $1 — выводим первый аргумент
       shift — удаляем первый аргумент, смещаем все аргументы
done — конец цикла
```

![3](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab12/report/image/3.jpg){#fig:003 width=70%}

![4](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab12/report/image/4.jpg){#fig:004 width=70%}

3. Написали командный файл — аналог команды ls (без использования самой этой команды и команды dir ). Он выдает информацию о нужном каталоге и выводит информацию о возможностях доступа к файлам этого каталога (рис. [-@fig:005], [-@fig:006]).

```
если не использовать команду ls или команду dir, то данную задачу легко выполнить с помощью команды find, если указать ей опцию поиска файлов с определенным правом доступа
```

![5](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab12/report/image/5.jpg){#fig:005 width=70%}

![6](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab12/report/image/6.jpg){#fig:006 width=70%}

4. Написали командный файл, который получает в качестве аргумента командной строки формат файла ( .txt , .doc , .jpg , .pdf и т.д.) и вычисляет количество таких файлов в указанной директории. Путь к директории также передаётся в виде аргумента командной строки (рис. [-@fig:007], [-@fig:008]).

```
ищем командой find в каталоге $1 (первый аргумент) файлы заканчивающиеся "*" на нужное расширение $2 (аргумент второй) передаем вывод | в команду подсчета wc с аргументом считающим слова -l
```

![7](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab12/report/image/7.jpg){#fig:007 width=70%}

![8](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab12/report/image/8.jpg){#fig:008 width=70%}

# Выводы

В данной работе мы изучили основы программирования в оболочке ОС UNIX/Linux. Научились писать небольшие командные файлы и скрипты на языке bush.

# Список литературы{.unnumbered}

1. [Операционные системы](https://esystem.rudn.ru/pluginfile.php/2586730/mod_resource/content/4/010-lab_shell_prog_1.pdf)
