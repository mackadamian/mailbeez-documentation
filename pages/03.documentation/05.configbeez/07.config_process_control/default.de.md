---
# http://learn.getgrav.org/content/headers
title: Prozess Kontrolle
slug: config_process_control
date: 26-03-2012
published: true
publish_date: 26-03-2012
# unpublish_date: 26-03-2012
template: docs
# theme: false
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: done
    category: [docs]
    tag: [core]
# added collection selector

author:
    name: admin
metadata:
    author: admin
---

Das Untersystem zur Prozess-Kontrolle stellt sicher, dass nur ein Versende-Prozess zur Zeit aktiv sein kann. Andernfalls kann es zu überlappenden Prozessen kommen, welche zum mehrfachen Versand der gleichen Emails führen kann.

>>>> Die Grundeinstellungen sollten nur geändert werden, wenn Sie die Auswirkungen verstehen!