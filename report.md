---
## Front matter
title: "Отчет по курсу"
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

Ознакомиться с функционалом операционной системы Linux.

# Задание

Просмотреть видео и на основе полученной информации пройти тестовые задания.

# Теоретическое введение

Линукс - в части случаев GNU/Linux — семейство Unix-подобных операционных систем на базе ядра Linux, включающих тот или иной набор утилит и программ проекта GNU, и, возможно, другие компоненты. Как и ядро Linux, системы на его основе, как правило, создаются и распространяются в соответствии с моделью разработки свободного и открытого программного обеспечения. Linux-системы распространяются в основном бесплатно в виде различных дистрибутивов — в форме, готовой для установки и удобной для сопровождения и обновлений, — и имеющих свой набор системных и прикладных компонентов, как свободных, так и проприетарных. 

# Выполнение лабораторной работы
## блок 1

![Задание 1](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/1.png){#fig:002 width=70%}

Курс действительно называется "Введение в Linux", поэтому с этим вопросом проблем не возникло.

![Задание 2](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/2.png){#fig:002 width=70%}

Прочитав критерии прохождения курса, я отметила необходимые утверждения.

![Задание 3](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/3.png){#fig:003 width=70%}

Стандартная операционная система, именно она стоит у меня на основном компьютере.



На свой компьютер мы устанавливали специальную программу VirtualBox, которая нужна для подключения одной операционной на другой.

![Задание 5](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/5.png){#fig:005 width=70%}

Да, моя виртуальная машина хорошо работает, и у меня получилось запустить с неё Линукс, но в последнее время я чаще использую ноутбук, на котором Линукс стоит как основная операционная система.

![Задание 6](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/6.png){#fig:006 width=70%}

Я создала документ, и перед сохранением выбрала нужный формат, а после я его прикрепила к курсу. Прикрепленный файл видно на скриншоте.

![Задание 7](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/7.png){#fig:007 width=70%}

deb — формат пакетов операционных систем проекта Debian. Используется также их производными, такими как Ubuntu, Knoppix и другими.


![Задание 8](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/8.png){#fig:008 width=70%}

Менеджер обновлений — это программа для обновления установленного программного обеспечения в дистрибутивах ОС Linux, основанных на Debian или использующих систему управления пакетами APT. Менеджер обновлений устанавливает обновления безопасности или просто улучшающие функциональность программы.

![Задание 9](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/9.png){#fig:009 width=70%}

Ассоль - героиня литературного произведения, а термин - это определение.

![Задание 10](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/10.png){#fig:010 width=70%}

![Задание 11](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/11.png){#fig:011 width=70%}

Интерфейс командной строки Linux является регистрозависимым, поэтому не подходит вариант, где буква А - маленькая(строчная).

![Задание 12](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/12.png){#fig:012 width=70%}

![Задание 13](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/13.png){#fig:013 width=70%}

rm -r удаление директории и рекуррентное удаление файлов, находящихся в ней.

![Задание 12](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/12.png){#fig:012 width=70%}

![Задание 13](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/13.png){#fig:013 width=70%}

![Задание 14](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/14.png){#fig:014 width=70%}

![Задание 15](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/15.png){#fig:015 width=70%}

![Задание 16](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/16.png){#fig:016 width=70%}

![Задание 17](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/17.png){#fig:017 width=70%}

![Задание 18](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/18.png){#fig:018 width=70%}

![Задание 19](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/19.png){#fig:019 width=70%}

![Задание 20](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/20.png){#fig:020 width=70%}

![Задание 21](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/21.png){#fig:021 width=70%}

![Задание 22](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/22.png){#fig:022 width=70%}

![Задание 23](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/23.png){#fig:023 width=70%}

![Задание 24](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/24.png){#fig:024 width=70%}

![Задание 25](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/25.png){#fig:025 width=70%}

![Задание 26](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/26.png){#fig:026 width=70%}

![Задание 27](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/27.png){#fig:027 width=70%}

? = один символ

alexey = маленькая буква

И файл должен быть jpeg, а не jpg

![Задание 28](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/28.png){#fig:028 width=70%}

Регистр - маленькая буква, слово - world, а не word

![Задание 29](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/29.png){#fig:029 width=70%}


## блок 2

![Задание 30](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/30.png){#fig:030 width=70%}

![Задание 31](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/31.png){#fig:031 width=70%}

![Задание 32](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/32.png){#fig:032 width=70%}

![Задание 33](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/33.png){#fig:013 width=70%}

![Задание 34](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/34.png){#fig:034 width=70%}

![Задание 35](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/35.png){#fig:015 width=70%}

![Задание 36](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/36.png){#fig:036 width=70%}

![Задание 37](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/37.png){#fig:037 width=70%}

![Задание 38](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/38.png){#fig:038 width=70%}

![Задание 39](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/39.png){#fig:39 width=70%}

![Задание 40](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/40.png){#fig:040 width=70%}


![Задание 43](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/43.png){#fig:043 width=70%}

![Задание 44](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/44.png){#fig:044 width=70%}

![Задание 45](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/45.png){#fig:045 width=70%}

![Задание 46](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/46.png){#fig:046 width=70%}

![Задание 47](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/47.png){#fig:047 width=70%}

![Задание 48](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/48.png){#fig:048 width=70%}

![Задание 49](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/49.png){#fig:49 width=70%}

![Задание 50](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/50.png){#fig:050 width=70%}

![Задание 51](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/51.png){#fig:051 width=70%}

![Задание 52](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/52.png){#fig:052 width=70%}

## блок 3

![Задание 53](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/53.png){#fig:053 width=70%}

![Задание 54](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/54.png){#fig:054 width=70%}

![Задание 55](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/55.png){#fig:055 width=70%}

![Задание 56](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/56.png){#fig:056 width=70%}

![Задание 57](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/57.png){#fig:034 width=70%}

![Задание 58](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/58.png){#fig:058 width=70%}

![Задание 59](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/59.png){#fig:059 width=70%}

![Задание 60](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/60.png){#fig:060 width=70%}

![Задание 61](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/61.png){#fig:061 width=70%}

![Задание 62](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/62.png){#fig:062 width=70%}

![Задание 63](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/63.png){#fig:063 width=70%}

![Задание 64](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/64.png){#fig:064 width=70%}

![Задание 65](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/65.1.png){#fig:065 width=70%}
![Задание 65](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/65.2.png){#fig:066 width=70%}

![Задание 66](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/66.1.png){#fig:067 width=70%}
![Задание 66](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/66.2.png){#fig:068 width=70%}

![Задание 67](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/67.png){#fig:069 width=70%}

![Задание 68](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/68.png){#fig:070 width=70%}

![Задание 69](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/69.png){#fig:071 width=70%}

![Задание 70](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/70.png){#fig:072 width=70%}

![Задание 71](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/71.1.png){#fig:073 width=70%}
![Задание 71](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/71.2.png){#fig:074 width=70%}

![Задание 72](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/72.1.png){#fig:075 width=70%}
![Задание 72](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/72.2.png){#fig:076 width=70%}

![Задание 73](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/73.png){#fig:077 width=70%}

![Задание 74](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/74.png){#fig:078 width=70%}

![Задание 75](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/75.png){#fig:079 width=70%}

![Задание 76](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/76.png){#fig:080 width=70%}

![Задание 77](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/77.png){#fig:081 width=70%}

![Задание 78](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/78.png){#fig:082 width=70%}

![Задание 79](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/79.1.png){#fig:083 width=70%}
![Задание 79](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/79.2.png){#fig:084 width=70%}

![Задание 80](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/80.png){#fig:085 width=70%}

![Задание 81](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/81.png){#fig:086 width=70%}

![Задание 82](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/82.png){#fig:087 width=70%}

![Задание 83](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/83.png){#fig:088 width=70%}

![Задание 84](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/84.png){#fig:089 width=70%}

![Задание 85](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/85.png){#fig:090 width=70%}

![Задание 86](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/86.png){#fig:091 width=70%}

![Задание 87](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/87.png){#fig:092 width=70%}

![Задание 88](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/88.png){#fig:093 width=70%}
 
Сертификат 
![сертификат](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/external_course/report/image/89.png){#fig:094 width=70%}

# Выводы

Я просмотрела курс и освежила в памяти навыки работы с более сложными командами в Линукс.


