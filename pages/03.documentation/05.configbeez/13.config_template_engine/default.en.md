---
title: 'Template Engine'
slug: config_template_engine
date: 26-03-2012
published: true
publish_date: 26-03-2012
template: docs
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: done
    category:
        - docs
    tag:
        - core
author:
    name: admin
metadata:
    author: admin
---

MailBeez utilizes the popular template system "[Smarty](http://smarty.net)" to generate email content.

Here you can empty the cache of the template system.

Not all email clients support external CSS files, so by default all CSS are converted into inline CSS. In case this causes issues with custom templates you can deactivate this behaviour.