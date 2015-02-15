---
last\_modified: 2015-02-15 10:39:42
tags: Perl
author: perlnews
title: Выпущен Perl 5.20.2
---

После 5 месяцев разработки выпущен второй корректирующий релиз стабильной
версии 20 Perl 5. Полный список изменений доступен в
[perldelta](https://metacpan.org/pod/release/SHAY/perl-5.20.2/pod/perldelta.pod).

---

Основные изменения:

* В новом релизе обновлён модуль `Data::Dumper`, в котором исправлена проблема
  [CVE-2014-4330](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-4330),
  приводящая к рекурсии при дампе глубоко вложенных структур данных.
* Исправлен [крах](https://rt.perl.org/Public/Bug/Display.html?id=123443) в
  `PerlIO::Sacalar` при задании файловой позиции за пределами скаляра.
* Появился новый документ
  [perlunicook](https://metacpan.org/pod/release/SHAY/perl-5.20.2-RC1/pod/perlunicook.pod),
  который содержит исчерпывающую информацию о работе с Юникодом в Perl.
* Восстановлена работоспособность сборки на платформах IRIX и Tru64
* Исправлены несколько ошибок assert в отладочных сборках Perl.
* Исправлен [крах](https://rt.perl.org/Ticket/Display.html?id=123495) при
  вызове gmtime() с параметром NaN.
* Исправлено [переполнение буфера и
  крах](https://rt.perl.org/Ticket/Display.html?id=123604) при компиляции
  определённых шаблонов в регулярных выражениях
* Устранена [утечка памяти](https://rt.perl.org/Ticket/Display.html?id=123198)
  в некоторых регулярных выражениях, появившаяся в Perl 5.20.1 

