---
## Front matter
title: "Отчёт по индивидуальному проекту"
subtitle: "Архитектура компьютеров и операционные системы"
author: "Мутале Чали"

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Быстрое развертывание сайта на GitHub Pages с помощью генератора статического html Hugo.

# Задание

- Установка программного обеспечения
- Установка темы
- Публикация сайта

# Выполнение лабораторной работы

## Установка программного обеспечения

Установливаю программу вручную с репозитория на Github:

![](image/1.png){#fig:001 width=70%}

Рис. 1: Установка Hugo

Распаковаю программу и копирую её в bin:

![](image/2.png){#fig:002 width=70%}

Рис. 2: Распаковка

По шаблону Academic-cv создаю новый репозиторий blog:

![](image/3.png){#fig:003 width=70%}

Рис. 3: blog
 
Клонирую репозиторий, который содержит структуру сайта в каталог work/blog :

![](image/4.png){#fig:004 width=70%}

Рис. 4: Клонирование

Перехожу в этот же каталог и проверяю с помощью ls -l:

![](image/5.png){#fig:005 width=70%}

Рис. 5: Проверка

## Установка темы

Запускаю hugo:

![](image/6.png){#fig:006 width=70%}

Рис. 6: Запуск hugo

Запускаю программу с командой server, чтобы видеть сайт на локальный сервер:

![](image/7.png){#fig:007 width=70%}

Рис. 7: hugo server

![](image/8.png){#fig:008 width=70%}

Рис. 8: Сайт на локальном сервере

Создаю еще один репозиторий имя, которое является адресом сайта:

![](image/9.png){#fig:009 width=70%}

Рис. 9: новый репозиторий

Клонирую созданный репозиторий, который храняется у себя в каталог wakutaipa.github.io:

![](image/10.png){#fig:0010 width=70%}

Рис. 10: Клонирование

Создаю новую ветку с именем main:

![](image/11.png){#fig:0011 width=70%}

Рис. 11: Новая ветка

## Публикация сайта

Создаю пустой файл readme.md и отправляю на глобальный репозиторий:

![](image/12.png){#fig:0012 width=70%}

Рис. 12: git push

Комментирую public с помощью mc в .gitignore чтобы каталоги с таким названием не игнорировались:

![](image/13.png){#fig:0013 width=70%}

Рис. 13: .gitignore

Добавляю репозиторий к каталогу с помощью git submodule add:

![](image/14.png){#fig:0014 width=70%}

Рис. 14: git submodule add

Запускаю hugo, чтобы заполнить созданный каталог:

![](image/15.png){#fig:0015 width=70%}

Рис. 15: Запуск hugo

Провеяю подключение между созданным каталогом и wakutaipa.github.io:

![](image/16.png){#fig:0016 width=70%}

Рис. 16: Проверка подключением

Далее отправляю все файлы на github:

![](image/17.png){#fig:0017 width=70%}

Рис. 17: Отправка файлы

![](image/18.png){#fig:0018 width=70%}

Рис. 18: Отправка файлы

![](image/19.png){#fig:0019 width=70%}

Рис. 19: github.io

# Выводы

При выполнении данной работы я научилась, как развмещать сайт на GitHub Pages с помощью генератора статического html Hugo.

# Список литературы{.unnumbered}

[Creating Hugo Site](https://yamadharma.github.io/ru/post/2022/04/12/creating-hugo-site/)
