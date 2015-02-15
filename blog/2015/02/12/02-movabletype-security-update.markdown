---
last\_modified: 2015-02-12 17:10:00
tags: security
author: perlnews
title: Вышли обновления безопасности MovableType 6.0.7 и 5.2.12
---

Вышли обновления, исправляющие ошибку в безопасности, для известной системы
управления контентом MovableType версии 6.0.7 и 5.2.12 (и в частности Movable
Type Open Source). Как указано в
[отчёте](https://movabletype.org/news/2015/02/movable_type_607_and_5212_released_to_close_security_vulnera.html)
уязвимости подвержены ветки 6.0.x и 5.2.x.

Уязвимость позволяла производить атаку LFI (_local file inclusion_ —
подключение локального файла) из-за использования модуля
[Storable](https://metacpan.org/pod/Storable) (метод thaw нельзя использовать
использовать на недоверенном контенте).

Как [отметили](http://www.openwall.com/lists/oss-security/2015/02/12/2) в
рассылке oss-security, уязвимость может быть легко использована и для
удалённого выполнения произвольного кода неаутентифицированным пользователем.
