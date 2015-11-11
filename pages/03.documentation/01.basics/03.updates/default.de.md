---
# http://learn.getgrav.org/content/headers
title: Aktualisieren des MailBeez Grundsystems
slug: updates
routes:
  default: /dokumentation/updates
  aliases:
    - /dokumentation/installation/config
menu: Aktualisieren
published: true
template: docs
# theme: false
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    category: docs
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


Ab Version 3.0 kann MailBeez sehr komfortabel mit dem integrierten Aktualisierungs-Programm auf die jeweils neueste Version gebracht werden.

## Aktualisieren bei Anzeige einer neuen Version

Die Versions-Kontrolle zeigt im System einen Hinweis an, wenn eine neue Version vorliegt. Bitte diesen Hinweis anklicken und dann das Aktualisierungs-Programm durchführen.

Das Aktualiserungs-Programm führt dabei folgende Schritte durch:

1. Prüfung der Server-Umgebung
1. Download der neuen Dateien
1. Prüfung, ob alle neuen Dateien geschrieben werden können - hierdurch wird sichergestellt, dass kein "Versions-Mix" von alten, nicht schreibbaren und neuen schreibbaren Dateien entstehen kann
1. Backup des /mailhive Verzeichnis
1. Schreiben der neuen Dateien (es werden alle Dateien überschrieben)


Nach Rückkehr zum MailBeez System sollten Sie einen entsprechenden Hinweis sehen.


>>>>>>Falls der Backup-Prozess nicht durchläuft, bitte mit Hilfe eines FTP Programmes alle Dateien deren Dateiname mit `appcache_` startet aus dem Verzeichnis `/mailhive/common/templates_c` löschen. Ab MailBeez Version 3.3.4 werden alte Cache Dateien automatisch entfernt.

## Manuelles Aktualisieren

In einigen Fällen kann es erforderlich sein, das Aktualisierungs-Programm manuell aufzurufen.

Hierzu bitte folgendes

`?cloudloader_mode=update_core` 

an die URL der MailBeez-Seite anhängen, also dass die URL im Browser etwa so aussieht:

`http://<shop-url>/<admin>/mailbeez.php?cloudloader_mode=update_core`

dann sollten Sie wie gewohnt durch den Aktualisierungs-Ablauf geführt werden.




## Aktualisierung per FTP

Sollte das Aktualisierungs-Programm aus unbekannten Gründen nicht durchlaufen, so kann das MailBeez Grundsystem auch "Old-School" per FTP aktualisiert werden:

Hierzu das
[MailBeez Grundsystem (.zip) downloaden](https://apps.mailbeez.com/api/public/v1/core/get), auf dem eigenen Rechner entpacken und dann per FTP auf den Server übertragen.