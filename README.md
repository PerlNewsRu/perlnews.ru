# Новостной сайт PerlNews.Ru

PerlNews.Ru -- это новостной блог о всех заметных событиях мира Perl на русском
языке.

## Как писать новости для сайта

Небольшая инструкция о том, как сделать свой вклад в развитие ресурса

Склонируйте репозиторий сайта

    $ git clone https://github.com/PerlNewsRu/perlnews.ru
    $ cd perlnews.ru

Установите Statocles

    $ cpanm Statocles

Добавить статью

    # новый бранч!
    $ git checkout -b "myname/news/branch"

    # сгенерить пост
    $ statocles blog post 01-post-uri-name

    # редактировать в формате Markdown
    $ vim blog/YYYY/MM/DD/01-post-uri-name.markdown

Пост с шапкой должен выглядеть, например так:

```
---
last\_modified: 2015-02-05 12:00:00
tags: темы, через, запятую
author: Имя Автора
title: Моя супер пупер новость
---

Тут идёт текст для затравки в формате Markdown

---

Тут под катом можно писать сколько душе угодно. Тоже в формате Markdown

```

Дальше генерим сайт и смотрим на 127.0.0.1:3000 что получилось. Редактируем и
повторяем шаги до идеального результата: 

    $ mkdir build

    # Генерим сайт
    $ statocles build

    # Локальный веб-сервер
    $ statocles daemon

Публикуем:

    $ git add blog
    $ git commit -m "my news"
    $ git push origin myname/news/branch

Затем делаем pull request.

Все тексты публикуются под лицензией [CC BY
4.0](http://creativecommons.org/licenses/by/4.0/deed.ru)
