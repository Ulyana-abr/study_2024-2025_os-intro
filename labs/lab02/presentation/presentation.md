---
## Front matter
lang: ru-RU
title: Научная презентация
subtitle: Дисциплина:Операционные системы
author:
  - Абрамова У. М.
institute:
  - Российский университет дружбы народов, Москва, Россия
  - Математический институт имени Никольского, Москва, Россия
date: 07.03.2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Абрамова Ульяна Михайловна
  * Студент НММбд-01-24
  * Российский университет дружбы народов
  * [1132246782@pfur.ru](mailto:1132246782@pfur.ru)
  * <https://github.com/Ulyana-abr>

:::
::: {.column width="30%"}


:::
::::::::::::::

# Вводная часть

## Актуальность

- Системы контроля версий (Version Control System, VCS) применяются при работе нескольких человек над одним проектом. 
- При внесении изменений в содержание проекта система контроля версий позволяет их фиксировать, совмещать изменения, произведённые разными участниками проекта, производить откат к любой более ранней версии проекта, если это требуется.

## Цели и задачи

- Изучить идеологию и применение средств контроля версий. Освоить умения по работе с git.

## Материалы и методы

- gh
- ssh key
- pgp key
- rephttps://github.com/yamadharma/course-directory-student-template

## Содержание исследования

1. Создание базовой конфигурации для работы с git
Устанавливаю git и gh (рис.1)

![установка git, gh](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/1.jpg){#fig:fig1 width=80%}

## Содержание исследования
Провожу базовую настройку git (рис.2)

![Настройка git](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/2.jpg){#fig:fig2 width=80%}

## Содержание исследования
2. Создание необходимых ключей
Создаю ssh (рис.3,4) и pgp ключи (рис.5)

![создание ssh ключа rba -b 4096](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/3.jpg){#fig:fig3 width=80%}

## Содержание исследования
![создание ssh ключа ed25519](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/4.jpg){#fig:fig4 width=80%}

## Содержание исследования
![создание pgp ключа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/5.jpg){#fig:fig5 width=80%}

## Содержание исследования
Создаю новую учетную запись  в github и добавляю туда ssh (рис.6) и pgp (рис.7) ключи

![добавление ssh ключа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/6.jpg){#fig:fig6 width=80%}

## Содержание исследования
![добавление pgp ключа](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/7.jpg){#fig:fig7 width=80%}

## Содержание исследования
3. Настройка подписей git и регистрация на Github
Настраиваю автоматические подписи коммитов git (рис.8), а также авторизируюсь в gh (рис.9) 

![Автоматические подписки комиков](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/8.jpg){#fig:fig8 width=80%}

## Содержание исследования
![авторизация](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/9.jpg){#fig:fig9 width=80%}

## Содержание исследования
4. Создание локального каталога для выполнения заданий по предмету
Создаю репозиторий курса (рис.10) 

![Репозиторий курса ](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/10.jpg){#fig:fig10 width=80%}

## Содержание исследования
Далее занимаюсь настройкой каталога, удаляя лишнее и создавая нужное
После чего отправляю файлы на сервер (рис.11) 

![отправка файлов на сервер](/home/umabramova/work/study/2024-2025/Операционные системы/os-intro/labs/lab02/presentation/image/11.jpg){#fig:fig11 width=80%}


## Результаты

- Я изучила идеологию и применение средств контроля версий, а также освоила умения по работе с git.

## Итоговый слайд

- Чем больше вы практикуетесь и пробуете новое, тем больше и чаще вы будете получать знаний и опыта в разных сферах

