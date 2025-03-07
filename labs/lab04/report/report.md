---
## Front matter
title: "Отчёт по лабораторной работе №4"
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

Получение навыков правильной работы с репозиториями git.

# Задание

1. Установка программного обеспечения
2. Практический сценарий использования git
3. Работа с репозиторием git 

# Выполнение лабораторной работы
## Установка программного обеспечения
Устанавливаю node js (рис.1)

![установка node js](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/1.jpg){#fig:fig1 width=80%}

Настраиваю node js (рис.2)

![настройка node js](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/2.jpg){#fig:fig2 width=80%}

Настраиваю конфигурацию общепринятых коммитов (рис.3)

![настройка общепринятых коммитов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/3.jpg){#fig:fig3 width=80%}

## Практический сценарий использования git

Создаю репозиторий git-extended (рис.4,5,6,7)

![подключение репозитория к github](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/51.jpg){#fig:fig51 width=80%}

![конфигурация общепринятых коммитов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/52.jpg){#fig:fig52 width=80%}

![изменение файла package.json](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/5.jpg){#fig:fig5 width=80%}

![отправка на github](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/6.jpg){#fig:fig6 width=80%}

Выполняю инициализацию git-flow, проверяю ветку и загружаю весь репозиторий в хранилище (рис.8)

![Конфигурация git-flow](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/7.jpg){#fig:fig7 width=80%}

Устанавливаю внешнюю ветку, как вышестоящую и создаю релиз с версией 1.0.0 , затем добавляю журнал изменений в индекс и заливаю релизную ветку в основную (рис.9)

![Конфигурация git-flow](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/8.jpg){#fig:fig8 width=80%}

## Работа с репозиторием git 
Разрабатываю ветку для новой функциональности (рис.10)

![создание ветки для новой функциональности](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/9.jpg){#fig:fig9 width=80%}

Создаю релиз с версией 1.2.3 (рис.11)

![создание релиза](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/10.jpg){#fig:fig10 width=80%}

Обновляю номер версии в package.json (рис.12)

![обновление номера версии](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/100.jpg){#fig:fig100 width=80%}

Создаю журнал изменений, добавляю его в индекс и отправляю данные на github (рис.13)

![Создание релиза git-flow](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/11.jpg){#fig:fig11 width=80%}

Создаю релиз с комментарием из журнала изменений (рис.14)

![Создание релиза с комментарием из журнала изменений](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab04/presentation/image/12.jpg){#fig:fig12 width=80%}

# Выводы

В итоге я получила навыки правильной работы с репозиториями git.

# Список литературы{.unnumbered}
1. [Операционные системы](https://esystem.rudn.ru/mod/page/view.php?id=1224234)
