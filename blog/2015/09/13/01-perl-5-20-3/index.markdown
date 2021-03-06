---
tags: Perl
author: perlnews
title: Выпущен Perl 5.20.3
---

После 7 месяцев разработки выпущен третий корректирующий релиз предыдущей
стабильной версии 20 Perl 5. Полный список изменений доступен в
[perldelta](https://metacpan.org/pod/release/SHAY/perl-5.20.3/pod/perldelta.pod).

---

Основные изменения:

* Поддержка сборки с помощью GCC 5, а также исправление ошибок сборки GCC 4.8 на
  платформе windows.
* Исправлен крах при обработке `eval { LABEL: }`.
* Исправлена проблема при использовании UTF-8 имён переменных в индексах
  массивов, UTF-8 строк для ограничителей встроенных документов.
* Устранено замедление при обработке регулярных выражений вида `/.*..../` и
  `/.*..../i`.
* Код вида `/$a[/` раньше начинал читать следующую строку кода, как если бы она
  шла сразу после открывающей скобки `[`. Это некорректное поведение некоторые
  использовали, например, в обфускации кода или создании
  [JAPH](https://ru.wikipedia.org/wiki/JAPH). Выяснилось, что в некоторых
  ситуациях этот баг мог приводить к краху, поэтому был исправлен.
* Исправлена фатальная ошибка, возникающая при попытке отлаживать
  Perl-программу, загружающую модуль `threads`/`threads::shared`.
