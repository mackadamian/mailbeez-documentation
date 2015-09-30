---
# http://learn.getgrav.org/content/headers
title: MailBeez Analytics
slug: config_analytics
routes:
    aliases:
        - /dokumentation/installation/config_queen/config_analytics
        
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


MailBeez Analytics ist das MailBeez eigene Analytics System, mit dem Sie den Erfolg Ihrer MailBeez Emails messen können.

Die Messung erfolgt nach folgenden Prinzipien:


### Öffnungsraten

eine Email gilt als geöffnet, wenn eines der folgenden Ereignisse eintrifft:

- Das Tracking-Pixel wird geladen (passiert nur, wenn das Email-Programm des Kunden die HTML-Version der Email anzeigt und die Bilder lädt)
- Klick auf einen Link in der Email, der zum Shop führt
- Tätigung eines Kaufes unter Nutzung des in der Email enthaltenen Gutschein-Codes


Das Lade des Tracking-Pixels verwendet einen Hoch-Performanten Aufruf, um die Server-Last zu minimieren: Jeder Pixel-Aufruf wird in einer Log-Datei protokolliert. Bei jeder Ausführung von MailBeez wird die Log-Datei in die MailBeez Analytics Datenbank importiert und die Log-Datei wird gelöscht. Hierdurch kann eine zeitliche Verzögerung zwischen dem eigentlichen Öffnen der Email und der Aktualisierung der Öffnungsraten entstehen.


### Klickraten

Eine Email gilt als angeklickt wenn das folgende Ereignis eintrifft:
- Klick auf einen Link in der Email, der zum Shop führt


### Bestellraten

Ein Bestellung gilt als über eine MailBeez Email vermittelt, wenn eine der folgenden Bedingungen erfüllt ist:

- Kauf als Folge eines Link-Klicks
- Kauf unter Nutzung des in der Email enthaltenen personalisierten Gutschein-Codes

>>>>> Öffnen und Klicks auf Kopie-Emails werden nicht gezählt, da diese Emails eine eigene Message-ID haben. Somit werden nur die Aktionen der wirklichen Empfänger (Kunden) erfasst.
