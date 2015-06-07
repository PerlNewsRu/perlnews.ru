---
tags: Perl, windows
author: perlnews
title: Выпущен Strawberry Perl 5.22.0.1
---

Выпущен релиз дистрибутива новой мажорной версии Perl для Windows _Strawberry
Perl_ 5.22.0.1.

Доступны msi-пакеты для установки:
[32-битной](http://strawberryperl.com/download/5.22.0.1/strawberry-perl-5.22.0.1-32bit.msi)
и
[64-битной](http://strawberryperl.com/download/5.22.0.1/strawberry-perl-5.22.0.1-64bit.msi)
версии.

Портабельные версии:
[32-битная](http://strawberryperl.com/download/5.22.0.1/strawberry-perl-5.22.0.1-32bit-portable.zip),
[64-битная](http://strawberryperl.com/download/5.22.0.1/strawberry-perl-5.22.0.1-64bit-portable.zip).

Новые версии содержат последнюю стабильную версию Perl 5.22.0. Кроме того, был
обновлен обновлён тулчейн gcc 4.9.2 и mingw-w64 v4.0.2. Полная информация о
релизах соотвественно
[32](http://strawberryperl.com/release-notes/5.22.0.1-32bit.html) и
[64](http://strawberryperl.com/release-notes/5.22.0.1-64bit.html).

К сожалению, msi-пакеты не подписаны, поэтому проверяйте [sha1
отпечаток](http://strawberryperl.com/releases.html).

На данный момент известно о нескольких проблемах в релизах: сломан модуль
`IPC::Run`, а в 64-битной сборке отсутствует `Math::Pari` вместе со всеми
зависимостями.
