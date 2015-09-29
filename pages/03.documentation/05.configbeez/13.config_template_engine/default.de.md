---
# http://learn.getgrav.org/content/headers
title: Template System
slug: config_template_engine
# menu: MailBeez Analytics
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
#      description: Your page description goes here
#      keywords: HTML, CSS, XML, JavaScript
#      robots: noindex, nofollow
#      og:
#          title: The Rock
#          type: video.movie
#          url: http://www.imdb.com/title/tt0117500/
#          image: http://ia.media-imdb.com/images/rock.jpg
#  cache_enable: false
#  last_modified: true
---

Zur Generierung der Emails nutzt MailBeez das beliebte Templatesystem "[Smarty](http://smarty.net)", welches auch in vielen Shop-Systemen zum Einsatz kommt.

In diesem Modul kann der Cache des Template Systemes geleert werden.

Nicht alle Email Programm unterstützen externe CSS Dateien, daher werden standardmässig alle CSS Angaben in Inline-CSS umgewandelt. Sollte dieses Verhalten bei selbst erstellten Email-Vorlagen stören, kann es hier deaktiviert werden.