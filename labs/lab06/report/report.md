---
## Front matter
title: "Отчет по лабораторной работе №6"
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

Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Задание

Выполнить действия, используя команды, такие как cd, mkdir, rm,  ls с различными опциями, man

# Выполнение лабораторной работы

Определяю полное имя моего домашнего каталога (рис. [-@fig:001]).

![Определение имя домашнего каталога](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/1.jpg){#fig:001 width=70%}

Перехожу в каталог /tmp и вывожу на экран содержимое данного каталога, используя команду  ls с различными опциями (-alF) (рис. [-@fig:002], [-@fig:003], [-@fig:004]).

![вывод содержимого каталога /tmp](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2.jpg){#fig:002 width=70%}

![вывод содержимого каталога /tmp](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/3.jpg){#fig:003 width=70%}

![вывод содержимого каталога /tmp](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/4.jpg){#fig:004 width=70%}

Таким образом, ls -a позволяет отобразить имена скрытых файлов, ls -l выводит на экран подробную информацию о файлах и каталогах, ls -F позволяет получить информацию о типах файлов (каталог, исполняемый файл, ссылка).


Определяю, есть ли в каталоге /var/spool подкаталог с именем cron (рис. [-@fig:005]).

![вывод содержимого каталога /var/spool](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/5.jpg){#fig:005 width=70%}

Перехожу в свой домашний каталог и вывожу на экран его содержимое с помощью команды ls. Далее, используя ту же команду, но уже с опцией -l, определяю, кто является владельцем файлов и подкаталогов (рис. [-@fig:006]).

![использование команды ls с опцией -l](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/6.jpg){#fig:006 width=70%}

В домашнем каталоге создаю новый каталог с именем newdir. Далее создаю в каталоге ~/newdir новый каталог с именем morefun (рис. [-@fig:007]).

![использование команды mkdir](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/7.jpg){#fig:007 width=70%}

В домашнем каталоге создаю одной командой три новых каталога с именами letters, memos, misk (рис. [-@fig:008]).

![использование команды mkdir](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/8.jpg){#fig:008 width=70%}

После чего удаляю эти каталоги одной командой (рис. [-@fig:009]).

![использование команды rmdir](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/9.jpg){#fig:009 width=70%}

Удаляю ранее созданный каталог ~/newdir командой rm. Проверяю, был ли каталог удалён  (рис. [-@fig:010]).

![использование команды ls](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/10.jpg){#fig:010 width=70%}

С помощью команды man определяю, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов, входящих в него (рис. [-@fig:011]).

![использование команды man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/11.jpg){#fig:011 width=70%}

С помощью команды man определяю набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов (рис. [-@fig:012]).

![использование команды man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/12.jpg){#fig:012 width=70%}

Использую команду man для просмотра описания следующих команд: cd, pwd, mkdir, rmdir, rm (рис. [-@fig:013], [-@fig:014], [-@fig:015], [-@fig:016], [-@fig:017]).

![использование команды man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/13.jpg){#fig:013 width=70%}

Основные опции команды cd:

-L - переходить по символическим ссылкам, данное поведение используется по умолчанию.
-P - разыменовывать символические ссылки. В данном случае, если осуществляется переход на символическую ссылку, которая указывает на директорию, то в результате команда cd изменит текущую рабочую директорию на директорию, указанную в качестве параметра (то есть ссылка будет разыменована).                 
-e - выдача ошибки, если папку, в которую нужно перейти, не удалось найти


![использование команды man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/14.jpg){#fig:014 width=70%}

Основные опции команды pwd:

-L (или --logical) - не разыменовывает символические ссылки, то есть, если путь содержит символические ссылки, то выводит их без преобразования в исходный путь.
-P (или --physical) - преобразовывает символические ссылки в исходные имена, то есть, если путь содержит символические ссылки, то они будут преобразованы в названия исходных директорий, на которые они указывают.
-help - отображает справку по команде pwd. 
-version - отображает версию утилиты pwd.


![использование команды man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/15.jpg){#fig:015 width=70%}

Основные опции команды mkdir:                                                                              

 -m или --mode - устанавливает права доступа для создаваемой директории. 
-p или --parents - создать все директории, которые указаны внутри пути. Если какая-либо директория существует, то предупреждение об этом не выводится.
-v или --verbose - выводить сообщение о каждой создаваемой директории.
-Z - установить контекст SELinux для создаваемой директории по умолчанию.
--context[=CTX] - установить контекст SELinux для создаваемой директории в значение CTX
--help - показать справку по команде mkdir
--version - показать версию утилиты mkdir


![использование команды man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/16.jpg){#fig:016 width=70%}

Основные опции команды rmdir:   
                                                                                                                              -ignore-fail-on-non-empty - не выводит сообщение об ошибке при попытке удаления непустого каталога. 
-p - удаляет каталог и его родителя из иерархии.
-v - выводит подробную информацию о выполнении команды. 
-help -  выводит текст справки. 
-version - указывает версию команды.


![использование команды man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/17.jpg){#fig:017 width=70%}

Основные опции команды rm:
-i - запрашивает подтверждение перед удалением каждого файла. 
-f - игнорирует ошибки и не запрашивает подтверждение удаления файлов. 
-r - рекурсивно удаляет каталоги и их содержимое.
-d - удаляет пустой каталог.
-v - показывает, что делает команда.


Используя информацию, полученную при помощи команды history, выполняю модификацию и исполнение команд из буфера команд (рис. [-@fig:018], [-@fig:019], [-@fig:020]).

![использование команды history](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/18.jpg){#fig:018 width=70%}

![выполнение модификации](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/19.jpg){#fig:019 width=70%}

![исполнение команд из буфера команд](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/20.jpg){#fig:020 width=70%}

# Выводы

В результате я приобрела практические навыки взаимодействия с системой посредством командной строки.

# Список литературы{.unnumbered}

1. [Операционные системы](file:///home/umabramova/Downloads/004-lab_shell.pdf)
