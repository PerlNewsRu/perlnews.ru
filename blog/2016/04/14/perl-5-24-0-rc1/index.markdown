---
tags: Perl
author: perlnews
title: Выпущен Perl 5.24.0-RC1
---
Не откладывая в долгий ящик, Рикардо Сигнес выпустил первый «настоящий»
релиз-кандидат новой мажорной версии Perl
[5.24.0-RC1](https://metacpan.org/release/RJBS/perl-5.24.0-RC1). Список
изменений по сравнению с Perl 5.22.0 доступен в
[perldelta](https://metacpan.org/pod/release/RJBS/perl-5.24.0-RC1/pod/perldelta.pod).
Среди основных изменений можно отметить:

* Постфиксное разыменование больше не экспериментальное, соответственно удалена
  поддержка авторазыменования.

* Поддержка стандарта Юникод 8.0.

* Удалена поддержка лексической переменной `my $_`.

* Оптимизирована процедура входа и выхода в/из область видимости, что ускоряет
  вызов функций, циклов и блоков кода.

* Прирост в скорости в регулярных выражениях с фиксированной строкой поиска за
  счёт использования соответствующей аппаратной поддержки.

* Множество исправлений ошибок.
