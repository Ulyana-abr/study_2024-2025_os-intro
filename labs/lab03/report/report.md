---
## Front matter
title: "Отчет по лабораторной работе №3"
subtitle: "Дисциплина: Операционные системы"
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
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью данной лабораторной работы является освоение процедуры оформления отчётов с помощью легковесного языка разметки Markdown.

# Задание

1. Заполнение отчета по выполнению лабораторной работы №3 с помощью языка разметки Markdown.
2. Выполнение заданий для самостоятельной работы.

# Теоретическое введение

Markdown - легковесный язык разметки, созданный с целью обозначения форматирования в простом тексте, с максимальным сохранением его читаемости человеком, и пригодный для машинного преобразования в языки для продвинутых публикаций. Внутритекстовые формулы делаются аналогично формулам LaTeX. В Markdown вставить изображение в документ можно с помощью непосредственного указания адреса изображения. Синтаксис Markdown для встроенной ссылки состоит из части [link text], представляющей текст гиперссылки, и части (file-name.md) – URL-адреса или имени файла, на который дается ссылка. Markdown поддерживает как встраивание фрагментов кода в предложение, так и их размещение между предложениями в виде отдельных огражденных блоков. Огражденные блоки кода — это простой способ выделить синтаксис для фрагментов кода.

# Выполнение лабораторной работы
## Заполнение отчета по выполнению лабораторной работы №3 с помощью языка разметки Markdown
Открываю терминал. Перехожу в каталог курса, сформированный при выполненнии прошлой лаборатной работы, и обновляю локальный репозиторий, скачав измения с помощью команды git pull (рис.1)

![Обновление локального репозитория](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/1.jpg){#fig:fig1 width=90%}

Далее перемещаюсь в каталог с шаблоном отчета по лабораторной работе №3 с помощью cd. Комплирую шаблон с использованием Makefile, вводя команду make (рис.2)

![Компилирование шаблона](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/2.jpg){#fig:fig2 width=80%}

Открываю сгенерированный файл report.docx, report.pdf (рис.3,4), тем самым убедившись,что все правильно сгенерировалось.

![Открытие файла docx](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/3.jpg){#fig:fig3 width=80%}

![Открытие файла pdf](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/4.jpg){#fig:fig4 width=80%}

Удаляю полученные файлы с использованием Makefile, вводя команду make clean (рис.5)

![Удаление файлов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/5.jpg){#fig:fig5 width=80%}

Открываю файл report.md с помощью текстового редактора gedit (рис.6)

![Открытие файла с помощью текстового редактора](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/6.jpg){#fig:fig6 width=80%}

Начинаю заполнять отчет с помощью языка разметки Markdown в скопированном файле (рис.7)

![Заполнение отчета](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/7.jpg){#fig:fig7 width=80%}

Компилирую файл и отправляю на GitHub (рис.8)

![Отправка файла на сайт](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/8.jpg){#fig:fig8 width=80%}

## Выполнение заданий для самостоятельной работы
Перехожу в директорию lab02/report с помощью cd, чтобы там заполнять отчёт по второй лаб.работе (рис.9)

![Премещение между директориями](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/9.jpg){#fig:fig9 width=80%}

Файл report.md открываю с помощью текстового редактора и начинаю заполнять (рис.10)

![Работа над отчётом](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/10.jpg){#fig:fig10 width=80%}

Компилирую файл с отчетом по лабораторной работе, добавляю изменения на GitHub с помощью команды git add и сохраняю изменения с помощью commit (рис.11)

![Отпрвка файлов на GitHub](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab03/presentation/image/11.jpg){#fig:fig11 width=80%}

# Выводы
В результате выполнения данной лабораторной работы я освоила процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Список литературы{.unnumbered}
1. [Операционные системы](https://esystem.rudn.ru/pluginfile.php/2586712/mod_resource/content/3/003-lab_markdown.pdf)
