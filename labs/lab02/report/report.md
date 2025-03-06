---
## Front matter
title: "Отчет по лабораторной работе №2"
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
Изучить идеологию и применение средств контроля версий. Освоить умения по работе с git.

# Задание

1. Создать базовую конфигурацию для работы с git.
   
    1.1. Создать ключ SSH.
    
    1.2. Создать ключ PGP.
    
    1.3. Настроить подписи git.
    
    1.4. Зарегистрироваться на Github.
    
    1.5. Создать локальный каталог для выполнения заданий по предмету.

# Выполнение лабораторной работы
## Создание базовой конфигурации для работы с git

Устанавливаю git и gh (рис.1)

![установка git, gh](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/1.jpg){#fig:fig1 width=80%}

Провожу базовую настройку git (рис.2)

![Настройка git](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/2.jpg){#fig:fig2 width=80%}

### Создание необходимых ключей
Создаю ssh (рис.3,4) и pgp ключи (рис.5)

![создание ssh ключа rba -b 4096](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/3.jpg){#fig:fig3 width=80%}

![создание ssh ключа ed25519](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/4.jpg){#fig:fig4 width=80%}

![создание pgp ключа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/5.jpg){#fig:fig5 width=80%}

Создаю новую учетную запись  в github и добавляю туда ssh (рис.6) и pgp (рис.7) ключи

![добавление ssh ключа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/6.jpg){#fig:fig6 width=80%}

![добавление pgp ключа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/7.jpg){#fig:fig7 width=80%}


### Настройка подписей git и регистрация на Github
Настраиваю автоматические подписи коммитов git (рис.8), а также авторизируюсь в gh (рис.9) 

![Автоматические подписки комиков](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/8.jpg){#fig:fig8 width=80%}

![авторизация](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/9.jpg){#fig:fig9 width=80%}

### Создание локального каталога для выполнения заданий по предмету
Создаю репозиторий курса (рис.10) 

![Репозиторий курса ](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/10.jpg){#fig:fig10 width=80%}

Далее занимаюсь настройкой каталога, удаляя лишнее и создавая нужное
После чего отправляю файлы на сервер (рис.11) 

![отправка файлов на сервер](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/11.jpg){#fig:fig11 width=80%}

# Выводы

Я изучила идеологию и применение средств контроля версий, а также освоила умения по работе с git.

# Список литературы{.unnumbered}

1. [Операционные системы](https://esystem.rudn.ru/mod/page/view.php?id=1224230)
