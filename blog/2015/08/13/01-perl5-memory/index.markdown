---
tags: Perl
author: perlnews
title: Потребление памяти в разных версиях Perl 5
---

[Рейни Урбан](https://twitter.com/Reini_Urban) привёл несколько любопытных
графиков, демонстрирующих потребление памяти в различных версиях Perl 5,
начиная с версии 5.6.

---

На данном графике видно насколько увеличивается потребление памяти Perl 5 с
каждым новым релизом:

<blockquote class="twitter-tweet" lang="en"><p lang="en" dir="ltr"><a
href="https://twitter.com/hashtag/perl5?src=hash">#perl5</a> releases memory
bloat -e0, &lt;5.8.8 even measured against debugging versions [massif on
darwin] <a
href="http://t.co/tJG2ycoFay">pic.twitter.com/tJG2ycoFay</a></p>&mdash; Reini
Urban (@Reini_Urban) <a
href="https://twitter.com/Reini_Urban/status/631002366934917120">August 11,
2015</a></blockquote>

Тот же график, но с загрузкой базовых модулей `Config`, `warnings`, `strict`:

<blockquote class="twitter-tweet" lang="en"><p lang="en" dir="ltr"><a
href="https://twitter.com/hashtag/perl5?src=hash">#perl5</a> releases memory
bloat with some base modules: -MConfig -Mwarnings -Mstrict -E0 <a
href="http://t.co/VQz0TWl3za">pic.twitter.com/VQz0TWl3za</a></p>&mdash; Reini
Urban (@Reini_Urban) <a
href="https://twitter.com/Reini_Urban/status/631056777619095552">August 11,
2015</a></blockquote>

График, демонстрирующий влияние улучшения поддержки Юникода в Perl 5 на
потребление памяти:

<blockquote class="twitter-tweet" lang="en"><p lang="en" dir="ltr"><a
href="https://twitter.com/hashtag/perl5?src=hash">#perl5</a> releases memory
bloat with unicode <a
href="http://t.co/ppFvWeCnxd">pic.twitter.com/ppFvWeCnxd</a></p>&mdash; Reini
Urban (@Reini_Urban) <a
href="https://twitter.com/Reini_Urban/status/631056960700465152">August 11,
2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

