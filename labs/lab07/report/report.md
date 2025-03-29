---
## Front matter
title: "Отчет по лабораторной работе №7"
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

Ознакомление с файловой системой Linux, её структурой, именами и содержанием
каталогов. Приобретение практических навыков по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке исполь-
зования диска и обслуживанию файловой системы.

# Задание

1. Выполнение примеров по различным темам 
2. Выполнение различных действий с файлами и каталогами 
3. Использование команды chmod с различными опциями 
4. Проделывание упражнений 
5. Использование команды man


# Выполнение лабораторной работы
## Выполнение примеров по различным темам 

Сначала делаю примеры по теме "копирование файлов и каталогов" (рис. [-@fig:001], [-@fig:002],[ -@fig:003], [-@fig:004], [-@fig:005]).

![копирование файла в текущем каталоге](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/1.jpg){#fig:001 width=70%}

![копирование нескольких файлов в каталог](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2.jpg){#fig:002 width=70%}

![копирование файлов в произвольном каталоге](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/3.jpg){#fig:003 width=70%}

![копирование каталогов в текущем каталоге](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/4.jpg){#fig:004 width=70%}

![копирование каталогов в произвольном каталоге](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/5.jpg){#fig:005 width=70%}

Затем по теме "перемещение и переименование файлов и каталогов" (рис. [-@fig:006], [-@fig:007],[ -@fig:008], [-@fig:009], [-@fig:010]).

![переименование файлов в текущем каталоге](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/6.jpg){#fig:006 width=70%}

![перемещение файлов в другой каталог](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/7.jpg){#fig:007 width=70%}

![переименование каталогов в текущем каталоге](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/8.jpg){#fig:008 width=70%}

![перемещение каталога в другой каталог](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/9.jpg){#fig:009 width=70%}

![переименование каталога, не являющегося текущим](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/10.jpg){#fig:010 width=70%}

Далее по теме "изменение прав доступа" (рис. [-@fig:011], [-@fig:012],[ -@fig:013], [-@fig:014])

![изменение прав доступа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/11.jpg){#fig:011 width=70%}

![изменение прав доступа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/12.jpg){#fig:012 width=70%}

![изменение прав доступа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/13.jpg){#fig:013 width=70%}

![изменение прав доступа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/14.jpg){#fig:014 width=70%}

## Выполнение различных действий с файлами и каталогами 
Копирую файл в домашний каталог и называю его equipment (рис. [-@fig:015])

![копирование и переименование](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/15.jpg){#fig:015 width=70%}

В домашнем каталоге создаю директорию, перемещаю ранее созданный файл в каталог, переименовываю его (рис. [-@fig:016])

![создание, перемещение и переименование](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/16.jpg){#fig:016 width=70%}

Создаю в домашнем каталоге файл abc1 и копирую его в созданный до этого каталог (рис. [-@fig:017])

![создание и копирование](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/17.jpg){#fig:017 width=70%}

В том же каталоге создаю каталог equipment, в который перемещаю файлы equiplist1, 2 (рис. [-@fig:018])

![создание и перемещение](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/18.jpg){#fig:018 width=70%}

В домашнем каталоге создаю каталог newdir, перемещаю его в использованный до этого каталог и задаю новое имя plans (рис. [-@fig:019])

![создание, перемещение и перименование](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/19.jpg){#fig:019 width=70%}

## Использование команды chmod с различными опциями 
Создаю нужные файлы и определяю какие опции chmod необходимы, чтобы присвоить файлам определенные права доступа (рис. [-@fig:020])

![опции команды chmod](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/20.jpg){#fig:020 width=70%}


## Проделывание упражнений 
С помощью команды cat просматриваю содержимое файла /etc/passwd (рис. [-@fig:021])

![просмотр содержимого файла](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/21.jpg){#fig:021 width=70%}

Копирую файл feathers в файл file.old, создаю каталог play (рис. [-@fig:022])

![копирование файла и создание каталога](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/22.jpg){#fig:022 width=70%}

Перемещаю каталог fun в каталог play и задаю новое имя games (рис. [-@fig:023])

![перемещение и переименование](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/23.jpg){#fig:023 width=70%}

Лишаю владельца файла feathers право на чтение (рис. [-@fig:024])

![команда chmod](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/24.jpg){#fig:024 width=70%}

В результате чего не получается не получается просмотреть файл командой cat, а также скопировать данный файл (рис. [-@fig:025])

![результат лишения права владельца на чтение](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/25.jpg){#fig:025 width=70%}

Лишаю владельца каталога play права на выполнение, из-за чего не получается перейти в него (рис. [-@fig:026])

![команда chmod](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/26.jpg){#fig:026 width=70%}

## Использование команды man
Использую команду man по командам mount, fsck, mkfs, kill (рис. [-@fig:027], [-@fig:028],[-@fig:029], [-@fig:030]).

![mount](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/27.jpg){#fig:027 width=70%}

Команда mount используется для монтирования файловой системы. Она принимает два параметра: файл устройства, соответствующий диску или разделу, на котором расположена файловая система, и имя каталога, к которому будет монтироваться система. Например, чтобы смонтировать дискету MS-DOS, нужно выполнить команду:

mount -t msdos /dev/fd0 /floppy


![fsck](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/28.jpg){#fig:028 width=70%}

Команда fsck служит для проверки целостности и работоспособности файловой системы. Большинство систем сконфигурировано так, что команда fsck запускается автоматически при загрузке системы. Например, чтобы проверить диск /dev/sda6, нужно выполнить команду:

sudo fsck -a /dev/sda6


![mkfs](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/29.jpg){#fig:029 width=70%}

Команда mkfs позволяет создать файловую систему Linux. Например, чтобы отформатировать раздел с файловой системой ext4, можно выполнить команды:

mkfs.ext4 /dev/sdb3


![kill](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/30.jpg){#fig:030 width=70%}

Команда kill используется для завершения процессов. Например, чтобы корректно завершить процесс с PID 98989, нужно выполнить команду:

kill -TERM 98989

# Выводы

В результате я ознакомилась с файловой системой Linux, приобрела практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами и по проверке использования диска и обслуживанию файловой системы

# Список литературы{.unnumbered}
1. [Операционные системы](https://esystem.rudn.ru/pluginfile.php/2586720/mod_resource/content/4/005-lab_files.pdf)
