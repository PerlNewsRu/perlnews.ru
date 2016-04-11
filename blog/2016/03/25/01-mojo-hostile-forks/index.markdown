---
tags: mojo, fork
author: perlnews
title: Враждебные форки
---

В документации Mojolicious появилось
[предостережение](https://github.com/kraih/mojo/blob/master/lib/Mojolicious/Guides/Contributing.pod#fork-policy)
от создания форков отдельных частей проекта Mojolicious, которые не были
одобрены разработчиками Mojolicious. Форки не только ведут к истощению ресурсов
проекта, бренда, но также лишают его возможных баг-репортов и патчей. В
качестве примеров можно привести
[DOM::Tiny](https://metacpan.org/pod/DOM::Tiny) , который является форком
[Mojo::DOM](https://metacpan.org/pod/Mojo::DOM), или
[JSON::Tiny](https://metacpan.org/pod/JSON::Tiny), который является форком
[Mojo::JSON](https://metacpan.org/pod/Mojo::JSON).
Например, [улучшение](https://github.com/daoswald/JSON-Tiny/pull/2) для
JSON::Tiny никто не удосужился предложить портировать обратно в Mojo::JSON, а
[улучшения](https://github.com/kraih/mojo/commit/7a65c82) в Mojo::JSON не
попадают в форк, таким образом складывается ситуация, когда оба проекта несут
потери.

Себастьян Ридель настроен серьёзно и уже поместил негативный
[отзыв](http://cpanratings.perl.org/dist/DOM-Tiny#12742) дистрибутиву
DOM-Tiny на cpanratings.
