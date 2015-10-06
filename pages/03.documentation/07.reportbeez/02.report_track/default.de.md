---
# http://learn.getgrav.org/content/headers
title: Auflistung Tracking Data
slug: report_track
# menu: Tracking Data
date: 03-03-2011
published: true
publish_date: 03-03-2011
# unpublish_date: 03-03-2011
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

>>>>>>Dieser Bericht kann schnell und kompfortable vom MailBeez Dashboard über den "Beez-O-Graph" geöffnet werden. Mit Klick auf die Legende **Emails versendet**, **geöffnet**, **geklickt** oder **bestellt** werden die entsprechenden Daten gefiltert angezeigt

MailBeez protokolliert jeden Email-Versand. Diese Tracking Daten werden verwendet, um sicherzustellen, dass jede Email nur genau 1x versendet wird - und verhinder damit den Mehrfach-Versand von Emails.

Als Bestandteil des Grund-Systemes gibt dieser Bericht auch einen guten Einblick, welche Emails versendet worden sind - und welche Aktionen vom Kunden getätigt wurden.

Der Bericht gibt auch Auskunft darüber, in welcher Betriebs-Art die Email versendet worden ist:

- **PROD**:  Abmeldung im Produktions-Modus
- **[SIM]**:  Abmeldung im Simulations-Modus

>>>>>Das Abmelden im Simulations-Modus wird nur dann richtig erfasst, wenn unter MailBeez > Konfiguration > Simulation die "Simulations-Protokollierung" aktiviert (True) ist.

Die Simulations-Daten können mit Klick auf "Simulation neu starten" gelöscht werden.