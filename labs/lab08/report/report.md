---
## Front matter
title: "Отчет по лабораторной работе №8"
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

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных. Приобретение практических навыков: по управлению процессами, по проверке использования диска и обслуживанию файловых систем.

# Задание

1. Осуществите вход в систему, используя соответствующее имя пользователя.
2. Запишите в файл file.txt названия файлов, содержащихся в каталоге /etc. Допи-
шите в этот же файл названия файлов, содержащихся в вашем домашнем каталоге.
3. Выведите имена всех файлов из file.txt, имеющих расширение .conf, после чего
запишите их в новый текстовой файл conf.txt.
4. Определите, какие файлы в вашем домашнем каталоге имеют имена, начинавшиеся
с символа c? Предложите несколько вариантов, как это сделать.
5. Выведите на экран (по странично) имена файлов из каталога /etc, начинающиеся
с символа h.
6. Запустите в фоновом режиме процесс, который будет записывать в файл ~/logfile
файлы, имена которых начинаются с log. Удалите файл ~/logfile.
7. Запустите из консоли в фоновом режиме редактор gedit. Определите идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep. Как ещё можно определить идентификатор процесса? Прочтите справку (man) команды kill, после чего используйте её для завершения процесса gedit.
8. Выполните команды df и du, предварительно получив более подробную информацию
об этих командах, с помощью команды man.
9. Воспользовавшись справкой команды find, выведите имена всех директорий, имею-
щихся в вашем домашнем каталоге.


# Выполнение лабораторной работы

1. Включаю компьютер и захожу в учетную запись. 
2. Далее записываю в файл file.txt названия файлов, содержащихся в каталоге /etc, и дописываю в этот же файл названия файлов, содержащихся в нашем домашнем каталоге (рис. [-@fig:001]).

![вывод и дописывание файлов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/1.jpg){#fig:001 width=70%}

3. Вывожу имена всех файлов из file.txt, имеющих расширение .conf, после чего записываю их в новый текстовой файл conf.txt (рис. [-@fig:002])

![вывод и записывание в новый текстовый файл](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2.jpg){#fig:002 width=70%}

4. С помощью команды find определяю, какие файлы в нашем домашнем каталоге имеют имена, начинавшиеся с символа c (рис. [-@fig:003]).

![вывод файлов с одинаковым первым символом](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/3.jpg){#fig:003 width=70%}

5. Вывожу на экран постранично имена файлов из каталога /etc, начинающиеся с символа h, также использую команду find (рис. [-@fig:004])

![постраничный вывод файлов](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/4.jpg){#fig:004 width=70%}

6. Запускаю в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log. Процесс выполнен. После этого удаляю файл ~/logfile, но сначала убиваю процесс в нем. (рис. [-@fig:005])

![Запуск в фоновом режиме процесса](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/5.jpg){#fig:005 width=70%}

7. Запускаю в фоновом режиме редактор gedit, Определили идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep.
Справка команды kill была получена и прочитана в предыдущей лабораторной работе, поэтому использую её для завершения процесса gedit. (рис. [-@fig:006])

![gedit в фоновом режиме](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/6.jpg){#fig:006 width=70%}

8. С помощью команды man получаю дополнительную информацию о командах df и du (рис. [-@fig:007], [-@fig:008])

![использование команды man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/7.jpg){#fig:007 width=70%}

![использование команды man](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/8.jpg){#fig:008 width=70%}

После чего выполняю данные команды (рис. [-@fig:009], [-@fig:010])

![выполнение df](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/9.jpg){#fig:009 width=70%}

![выполнение du](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/10.jpg){#fig:010 width=70%}

9. Воспользовавшись справкой команды find, вывожу имена всех директорий, имеющихся в нашем домашнем каталоге.  (рис. [-@fig:011])

![вывод директорий домашнего каталога](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/11.jpg){#fig:011 width=70%}

# Выводы

В данной работе я ознакомилась с инструментами поиска файлов и фильтрации текстовых данных. А также приобрела практические навыки по управлению процессами.

# Список литературы{.unnumbered}

1. [Операционные системы](https://esystem.rudn.ru/pluginfile.php/2586722/mod_resource/content/4/006-lab_proc.pdf)
