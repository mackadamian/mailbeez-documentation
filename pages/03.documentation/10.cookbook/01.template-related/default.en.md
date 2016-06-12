---
# http://learn.getgrav.org/content/headers
title: email template recipes
#menu: Beez-O-Graph
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


## Date format

### Issue

Dates are not formatted like they should

### Solution

#### Option 1

Dates are formatted according to the server configuration.

Please adjust the "locale" setting of your server, you will find more information on [php.net/strftime](http://php.net/strftime)

#### Option 2

Thanks to the [Smarty Date-Modifiers](http://www.smarty.net/docs/en/language.modifier.date.format.tpl) you can tweak the dates to your needs, e.g.:

```
{$coupon_expire|date_format:"%A, %B %e %Y"}
```

outputs

```
Monday, 1. December 2021
```



You find more information on [Smarty Date-Modifiers](http://www.smarty.net/docs/en/language.modifier.date.format.tpl).