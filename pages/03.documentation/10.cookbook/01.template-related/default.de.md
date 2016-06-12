---
# http://learn.getgrav.org/content/headers
title: Email Vorlagen Rezepte
#menu: Beez-O-Graph
slug: email-vorlagen
date: 17-02-2016
published: true
publish_date: 17-02-2016
template: tutorial
# theme: false
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: done
    category: [docs]
    tag: []
---

[TOC]


## Datums-Formatierung

### Problem

Datums-Angaben werden nicht im gewünschten Format dargestellt.

### Lösung

#### Möglichkeit 1
Datums-Angaben werden standardmässig anhand der Server-Konfiguration ausgegeben.

Bitte konfigurieren Sie die "locale" Einstellungen Ihres Servers, mehr Informationen hierzu finden Sie auf [php.net/strftime](http://php.net/strftime)

#### Möglichkeit 2

Mit Hilfe des [Smarty Datum-Modifiers](http://www.smarty.net/docs/en/language.modifier.date.format.tpl) können Sie die Datums-Ausgaben nach Ihren Wünschen anpassen. Dies kann z.B. so aussehen:
```
{$coupon_expire|date_format:"%A, %B %e %Y"}
```

liefert

```
Montag, 1. Dezember 2021
```



Weitere Informationen hierzu finden Sie auf [Smarty Datum-Modifiers](http://www.smarty.net/docs/en/language.modifier.date.format.tpl)