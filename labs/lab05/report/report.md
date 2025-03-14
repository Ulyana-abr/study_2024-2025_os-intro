---
## Front matter
title: "Отчет по лабораторной работе №5"
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

Целью данной лабораторной работы является настройка интерфейса с броузером, управление файлами конфигурации, использование chezmoi

# Задание

1. Настройка интерфейса с броузером
2. управление файлами конфигурации
3. использование chezmoi

# Выполнение лабораторной работы

Устанавливаю pass и gopass (рис.1,2)

![установка pass](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/1.jpg){#fig:fig1 width=80%}

![установка gopass](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2.jpg){#fig:fig2 width=80%}

Просматриваю список ключей (рис.3)

![просмотр списка ключей](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/3.jpg){#fig:fig3 width=80%}

Инициализирую хранилище (рис.4)

![инициализация хранилища](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/4.jpg){#fig:fig4 width=80%}

Создаю структуру git (рис.5)

![создание структуры ](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/5.jpg){#fig:fig5 width=80%}

Создаю новый репозиторий, задаю адрес репрозитория на хостинге, и затем выполняю синхронизацию (рис.6)

![создание и синхронизация нового репрозитория ](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/6.jpg){#fig:fig6 width=80%}

Устанавливаю browserpass (рис.7)

![установка browserpass](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/8.jpg){#fig:fig8 width=80%}

Образую пароль в ранее созданном файле (рис.8)

![создание пароля](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/7.jpg){#fig:fig7 width=80%}

Устанавливаю по и шрифты (рис.9, 10)

![установка необходимого по](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/9.jpg){#fig:fig9 width=80%}

![установка шрифтов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/10.jpg){#fig:fig10 width=80%}

Устанавливаю chezmoi и создаю свой репозиторий для конфигурационных файлов на основе шаблона (рис.11, 12)

![установка chezmoi](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/11.jpg){#fig:fig11 width=80%}

![создание репозитория](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/12.jpg){#fig:fig12 width=80%}

Подключаю репозиторий к своей системе (рис.13)

![подключение репозитория](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/13.jpg){#fig:fig13 width=80%}

Проверяю внесённые изменения и соглашаюсь с ними (рис.14)

![просмотр внесенных изменений](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/14.jpg){#fig:fig14 width=80%}

ежедневные операции с chezmoi (рис.15, 16)

![извлечение последних изменений](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/15.jpg){#fig:fig15 width=80%}

![автоматическая фиксация изменений и их отправка](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/16.jpg){#fig:fig16 width=80%}


# Выводы

В результате я выполнила настройку интерфейса с броузером, произвела управление файлами конфигурации и использовала chezmoi

# Список литературы{.unnumbered}

1. [Операционные системы](https://esystem.rudn.ru/mod/page/view.php?id=1224236#orgb06553f)
