---
last\_modified: 2015-02-10 08:29:17
tags: CPAN, facepalm
author: perlnews
title: В Pod::Simple по умолчанию будет кодировка CP-1252
---

Дэвид Уилер
[анонсировал](http://www.nntp.perl.org/group/perl.perl5.porters/2015/02/msg225550.html),
что в следующем релизе [Pod::Simple](https://metacpan.org/release/Pod-Simple)
(парсер POD-документации, используемый в том числе для perldoc) будет изменена
кодировка по-умолчанию с Latin-1 на CP-1252. Утверждается, что это будет
особенно полезно для POD-документов, созданных на платформе Windows, где эта
кодировка и встречается. Соответствующие изменения будут внесены и в
спецификацию POD Perl.
