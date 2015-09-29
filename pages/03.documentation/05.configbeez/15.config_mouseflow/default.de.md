---
# http://learn.getgrav.org/content/headers
title: Mouseflow Integration
slug: config_mouseflow
# menu: Mouseflow Integration
date: 20-10-2011
published: true
publish_date: 20-10-2011
# unpublish_date: 20-10-2011
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

## Was ist [Mouseflow](http://shrsl.com/?~6plv)?

[Mouseflow](http://shrsl.com/?~6plv) ist ein web service welcher das Verhalten der Besucher Ihrer Seite aufzeichnet und visuell Hinweis gibt, welche Bereiche am meisten Aufmerksamkeit erhalten. Unbeachtete Bereiche können verbessert werden, um mehr Aufmerksamkeit zu bekommen.

Die Daten werden als aussagekräftige “Wärmebilder” präsentiert. Zudem zeichnet [Mouseflow](http://shrsl.com/?~6plv) das Verhalten der Besucher auf – fast wie mit einer Videokamera. Dies ist enorm hilfreich, um die Benutzerfreundlichkeit der Seite zu untersuchen und zu sehen, wie Besucher auf Ihren Seiten navigieren.

Alles steht in Echtzeit zur Verfügung. Das kostenlose Paket erlaubt die Aufzeichnung des Verhaltens von monatlich bis zu 100 Besuchen auf und die Daten werden für 1 Monat gespeichert.

### Funktionen:

- **Folge alle Maus-Bewegungen, Clicks, Scrollen der Seite, Tastatureingaben und Ausfüllen von Formularen.**
- Entdecken Sie, welche Bereiche Ihrer Seite Schwierigkeiten bereiten und lernen Sie anhand der Beobachtungen, wie Sie diese verbessern können.
- Ein visueller Überblick zeigt die Clicks auf Ihren Seiten.
- Vergleichen Sie “Wärmebilder” verschiedener Zeiträume, um die Auswirkungen von Änderungen zu sehen.
- und [vieles mehr…](http://shrsl.com/?~6plv)

**Lesen Sie mehr über [alle Funktionen von Mouseflow](http://shrsl.com/?~6plv)**  
 Jetzt auf [Mouseflow](http://shrsl.com/?~6plv) registrieren und **Sie erhalten monatlich 100 Aufzeichnungen gratis**.

Mouseflow ist recht preisgünstig und daher auch für Klein-Unternehmer ideal, z.B. kostet die Aufzeichnung von 10.000 monatlichen Besuchen nur 49Eur/Monat

 

## Optimieren Sie Ihren Shop und MailBeez mit Mouseflow

Nach dem Einfügen des folgenden PHP Codes in die Datei `includes/application_bottom.php`  brauchen Sie nur noch den Tracking Code zu konfigurieren..


```
// MailBeez
if (defined('MAILBEEZ_MOUSEFLOW_STATUS') && MAILBEEZ_MOUSEFLOW_STATUS == 'True') {
    require_once(DIR_FS_CATALOG . 'mailhive/configbeez/config_mouseflow/includes/mouseflow_inc.php');
}
// - MailBeez
    
```

Zusätzlich erhalten Sie mit folgenden Konfigurationsmöglichkeiten Kontrolle darüber, welche Art von Besuchen Sie aufzeichnen wollen:

- Mouseflow aktivieren / deaktivieren
- Besucher aus MailBeez Kampagnen einbeziehen oder ausschliessen
- die Aufzeichung NUR auf Besucher aus MailBeez Kampagnen begrenzen
- Administratoren über IP-Adresse von der Aufzeichnung ausschliessen

Somit wird es also möglich, mit einer “kostenbewussten” Konfiguration lediglich Besucher aus MailBeez Kampagnen zu beobachten und die Webseiten danach zu optimieren:

- Welche Schritte führt ein Kunde bei Bitte um Bewertung durch?
- Wie verhalten sich Kunden beim Versuch der Rückgewinnung?
- Welchen Einfluss haben Gutscheine in den Emails?

Dies erlaubt Ihnen dann, Ihre MailBeez Kampagnen und Ihren Online-Shop zu Verbessern und die Ergebnisse von MailBeez zu optimieren!
