---
# http://learn.getgrav.org/content/headers
title: Shopauskunft Bewertungen in Emails
slug: filter_add_shopauskunft_feed
# menu: Shopauskunft Bewertungen in Emails
date: 03-05-2011
published: true
publish_date: 03-05-2011
# unpublish_date: 03-05-2011
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

Fügen Sie Ihre wertvollen Shopauskunft ratings automatisch in Ihre MailBeez Email Kampagnen ein – hervorragend um die Emails zur “Kundenrückgewinnung” (Winback) und “Kunden ohne Kauf” (Nopurchase) aufzuwerten.

Dieses Hilfsmodule ist Teil der [Shopauskunft Integration Suite](/documentation/configbeez/config_shopauskunft_rss_importer/?lang=de "Shopauskunft Integration Suite").

Mit der beiliegenden Standard Vorlage sehen die Bewertungen folgendermassen aus:

[![](http://www.mailbeez.com/wp-content/uploads/2011/05/default_email_template-300x289.png "default_email_template")](http://www.mailbeez.com/wp-content/uploads/2011/05/default_email_template.png)Default Template for Email Integration

 

 

### Optionen:

**Anzahl Bewertungen**  
 Anzahl Bewertungen in den Emails (Zahl)

**Mindestanzahl Sterne**  
 Nur Bewertungen mit mindestens diese Anzahl Sterne anzeigen (3-5)

**Zufällige Reihenfolge**  
 Zufällige Reihenfolge True) oder chronologische Reihenfolge (False)

 

### Anwendung:

Modul installieren und Aktvieren – vorher den Shopauskunft RSS feed Importer konfigurieren und testen.

Mit folgende Platzhaltern können Sie die konfigurierte Anzahl an Bewertungen in von MailBeez generierten Emails einfügen. Die Platzhalter können an jeder beliebigen Stellen in den MailBeez Vorlagen (\*.tpl Dateien) eingefügt werden. Sollen die Bewertungen in allen Emails sichtbar sein, am besten in die Hauptvorlage einfügen

Platzhalter für die HTML-Version der Vorlage:

> `{$content.rss.Shopauskunft.html}`

Platzhalter für die TXT-Version der Vorlage:

> `{$content.rss.Shopauskunft.txt}`

Die Vorlage für die Darstellung der Bewertungen ist folgende Datei

> `rss_email_html.tpl`  
> `rss_email_txt.tpl`

welche in folgendem Ordner liegt:

> `mailhive\configbeez\config_Shopauskunft_rss_importer\templates`

Fortgeschrittene Benutzter können auch das Daten-Object mit den Bewertungen direkt im Email Template verwenden – Anleitung hierzu finden Sie im Modul (Admin)
