---
title: Simulation
slug: config_simulation
date: 28-09-2015
published: true
template: docs
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: done
    category: [docs]
    tag: [core]
author:
    name: admin
metadata:
    author: admin
---

MailBeez unterscheidet grundsätzlich zwischen den Betriebsarten:

1. **Simulation**
2. **Produktion**


### Simulation [SIM]

Der Simulations-Modus ist gedacht, um - schwer zu erraten - die Funktion des MailBeez-Systemes anhand von Simulationen zu testen. Im Simulations-Modus arbeiten alle Module wie im Produktions-Modus, ABER: alle E-Mails werden nur an die hier hinterlegte E-Mail-Adresse versendet und NICHT an die Kunden!
Zur Kennzeichnung von Simulations-E-Mails wird die Kennung [SIM] z.B. im E-Mail-Betreff und im Gutschein-Code verwendet.

Beim Neustart einer Simulation werden alle Simulations-Daten gelöscht.


### Produktion

Wenn Sie mit den Ergebnissen der Simulations-Durchläufen zufrieden sind, können Sie beruhigt in die Betriebsart "Produktion" wechseln. Beim Ausführen der Module werden dann die E-Mails generiert und an die Kunden versendet.
