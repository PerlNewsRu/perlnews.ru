---
last\_modified: 2015-02-10 11:03:42
tags: Perl
author: perlnews
title: В библиотеке libc Apple использовался Perl для реализации wordexp
---

HackerNews сегодня [повторил](https://news.ycombinator.com/item?id=9025572) уже
мелькавшую новость о том, что по крайне мере до 2011 года в реализации функции
[`wordexp()`](http://pubs.opengroup.org/onlinepubs/9699919799/functions/wordexp.html)
в библиотеке libc Apple использовался Perl, как внешняя программа, производящая
разбор аргументов и собирающая их в строку с разделителем нуль-символом `\0`:

    char *cmd = "/usr/bin/perl -e 'print join(chr(0), @ARGV), chr(0)' -- ";

Оригинальный исходный код можно увидеть
[здесь](https://github.com/Apple-FOSS-Mirror/Libc/blob/2ca2ae74647714acfc18674c3114b1a5d3325d7d/gen/wordexp.c#L192).
