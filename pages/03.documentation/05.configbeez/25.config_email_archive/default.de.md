---
# http://learn.getgrav.org/content/headers
title: Email Web-Ansicht und Archiv
slug: config_email_archive
# menu: Email Web-Ansicht und Archiv
date: 28-04-2014
published: true
publish_date: 28-04-2014
# unpublish_date: 28-04-2014
template: docs
# theme: false
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: review
    category: [docs]
    tag: []
module:
    code: 'config_email_archive'
    category: [configbeez]
    compatiblity: [comp_osc,comp_cre,comp_digi,comp_zencart,comp_xtc,comp_gambio]
    thumbnail: 'http://www.mailbeez.com/wp-content/uploads/downloads/thumbnails/2014/04/icon_32.png'
    pro: 'pro'
    cert: 'true'
    price: '79 EUR'
    title_en: 'Web-View and Email Archive'
    teaser_en: 'Enrich you MailBeez Emails with a web-view and archive them'
    title_de: 'Email Archiv und Web-Ansicht'
    teaser_de: 'Erweitern Sie Ihre MailBeez-Emails mit einer Web-Ansicht und archivieren Sie diese.'
    author: 'MailBeez.com'
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

Mit dem Modul "Email Web-Ansicht und Archiv" erweitern Sie Ihr MailBeez System schnell und einfach um folgende Funktionen

## Web-Ansicht

Platzieren Sie den neuen Platzhalter

 
    <a href="{$webversion_url}">Web-Ansicht</a>


in Ihrer Haupt- oder auch Inhalts-Vorlage. Der Empfänger wird dann mit Klick auf diesen Link auf eine Web-Seite geleitet, welche die Email als Online-Version zeigt.

## Archiv

Alle Emails werden automatisch in Text- und HTML-Version archiviert und sind komfortable über den Beez-O-Graph aber auch je Kunden im kostenfreien [BeezDesk Kunden Insight](/dokumentation/configbeez/config_customer_insight/) einsehbar - So ist leicht nachvollziehbar, welche Emails den Kunden gesendet worden sind.

## Für die nächste Version geplante Funktionen

- erneuter Versand von archivierten Emails
- Optionale Teilen-Funktion der Web-Version
V1.0
- initial public version