---
## Front matter
title: "Отчет по лабораторной работе №1"
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину,
настройки минимально необходимых для дальнейшей работы сервисов.

# Заданиe

1. Установка Linux на Virtualbox
2. Настройки после установки
3. Установка программного обеспечения для создания документации
4. Выполнение заданий для самостоятельной работы


# Выполнение лабораторной работы
## Установка Linux на Virtualbox
Virtualbox был установлен в прошлом семестре, поэтому перейдем к созданию виртуальной машины (рис.1,2)

![создание виртуальной машины](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/1.jpg){#fig:fig1 width=80%}

![создание виртуальной машины](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/2.jpg){#fig:fig2 width=70%}

## Настройки после установки
После установки виртуальной машины, вхожу в OC под заданной при установке учетной записью и устанавливаю драйвера для Virtualbox (рис.3)

![установка драйверов для Virtualbox](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/3.jpg){#fig:fig3 width=80%}

Обновляю пакеты (рис.4)

![обновление пакетов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/4.jpg){#fig:fig4 width=70%}

Устанавливаю программу для удобства работы в консоли (рис.5)

![повышение комфорта работы](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/5.jpg){#fig:fig5 width=80%}

Настраиваю автоматическое обновление (рис.6)

![автоматическое обновление](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/6.jpg){#fig:fig6 width=80%}

И отключаю SELinux (рис.7)

![замена значения](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/7.jpg){#fig:fig7 width=70%}

 Далее настраиваю раскладку клавиатуры (рис.8)

![настройка раскладки клавиатуры](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/8.jpg){#fig:fig8 width=80%}

## Установка программного обеспечения для создания документации  
Запустив терминальный мультиплексор tmux и переключившись на роль супер-пользователя, устанавливаю с помощью менеджера пакетов pandoc и pandoc-crossref для работы с языком разметки Markdown (рис.9) , а также дистрибутив TeXlive (рис.10)

![Установка pandoc, pandoc-crossref](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/9.jpg){#fig:fig9 width=80%}

![установка texlive](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/10.jpg){#fig:fig10 width=80%} 

## Выполнение заданий для самостоятельной работы
Выполняя команду dmesg | grep -i “то,что ищем”, получаю информацию о версии ядра Linux, частоте и модели процессора, объеме доступной оперативной памяти, типе обнаруженного гипервизора и файловой системы корневого раздела и последовательности монтирования файловых систем (рис.11,12)

![Выполнение команд dmesg | grep -i “то,что ищем”](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/11.jpg){#fig:fig11 width=80%}

![Выполнение команд dmesg | grep -i “то,что ищем”](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab01/presentation/image/12.jpg){#fig:fig12 width=80%}

# Выводы

Я приобрела практические навыки установки операционной системы на виртуальную машину и настройки минимально необходимых для дальнейшей работы сервисов.

# Список литературы{.unnumbered}

[Операционные системы](https://esystem.rudn.ru/mod/page/view.php?id=1224227)
