---
last\_modified: 2015-02-11 11:03:06
tags: Perl
author: perlnews
title: Проблемы со сборкой Perl 5 с помощью GCC 5
---

RedHat, стоящий на острие разработки, провёл тестовую пересборку всех пакетов в
Fedora Rawhide с помощью новейшей версии компилятора GCC 5. По
[результатам](https://lists.fedoraproject.org/pipermail/devel/2015-February/207549.html)
пересборки выявились некоторые пакеты, которые этого не пережили, в том числе и
Perl 5.20.1.

Как выяснил Petr Pisar, это произошло вследствие изменений в выводе
препроцессора, из-за чего перестал правильно генерироваться `Errno.pm`.
[Патч](https://rt.perl.org/Public/Bug/Display.html?id=123784) уже доступен,
хотя, скорее всего, он уже не успевает попасть в грядущий релиз Perl 5.20.2.
