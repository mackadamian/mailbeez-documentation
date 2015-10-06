---
# http://learn.getgrav.org/content/headers
title: Ereignis Protokoll
slug: report_event_log
# menu: MailBeez Event Log Viewer
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

Das MailBeez System protokolliert eine Reihe von Aktivitäten, z.B. wann der Versende-Prozess gestartet wurde, ob es sich um eine Simulation, einen Test oder einen Aufruf im Produktions-Modus handelt.

Mit Hilfe des Ereignis-Protokolles können Sie einsehen, wie MailBeez arbeitet.

In der Spalte "Modus" können Sie sehen:
- **PROD** - MailBeez wurde im Produktions-Modus ausgeführt
- **[SIM]** - MailBeez wurde im Simulations-Modus ausgeführt

**Ereignisse**

- **MAILHIVE_RUN_INIT** – Initialisierung des MailBeez Versende-Prozesses. ein INIT ohne einen dazugehörigen COMPLETE Eintrag bedeutet, dass etwas schief gelaufen ist
- **MAILHIVE_RUN_COMPLETE**: Die Ausführung des Versende-Prozesses wurde sauber abgeschlossen
- **MAILHIVE_TEST_INIT**: Initialisierung des MailBeez Versende-Prozesses zum Versand einer Test-Email. Ein INIT ohne einen dazugehörigen COMPLETE Eintrag bedeutet auch hier, dass etwas schief gelaufen ist
- **MAILHIVE_TEST_COMPLETE**: Die Ausführung des Versende-Prozesses zum Test-Versand wurde sauber abgeschlossen
- **MAILBEEZ_MODULE_INIT**: Initialisierung eines Modules (Wenn das Ereignis-Protokoll so konfiguriert wurde)


Die weiteren Angaben des Protokolles sollten sich selbst erklären.