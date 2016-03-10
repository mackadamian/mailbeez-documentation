---
# http://learn.getgrav.org/content/headers
title: MailBeez Konfiguration einfach
slug: mailbeez-konfiguration-einfach
# menu: MailBeez Konfiguration einfach
date: 16-07-2012
published: true
publish_date: 16-07-2012
# unpublish_date: 16-07-2012
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
    name: kelly
metadata:
    author: kelly
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

Dieses Tutorial wird Ihnen helfen, das MailBeez System schnell zu konfigurieren. Wenn Sie lieber gleich etwas mehr Zeit investieren wollen, nutzen Sie Bitte das Tutorial “[MailBeez Konfiguration ausführlich](/dokumentation/tutorials/mailbeez-konfiguration-ausfuehrlich/)“, welches etwa 15-30Minuten in Anspruch nimmt.

Die hier verwendeten Screenshots wurden mit ZenCart erstellt. Auf anderen Shop-System wird das Admin-Interface etwas anders aussehen, der Aufbau und die Bedienkonzepte sind aber einheitlich für alle Platformen – soweit nicht ausdrücklich auf Abweichungen hingewiesen wird.

## Los gehts:

Öffnen Sie das MailBeez System in der Shop-Administration und klicken Sie auf den “Konfiguration” Reiter. Sie werden eine Reihe von Konfigurations-Gruppen sehen:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/common_images/config_tab.png&w=270&h=134&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.de/images/doc/common_images/config_tab.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In diesem Tutorial werden wir lediglich die beiden wichtigsten Konfigurations-Gruppen betrachten, um schnell einen ersten Test durchführen zu können: Die MailHive Grundeinstellungen und die Simulations-Einstellungen.

## Grundeinstellungen

Die 9 Einstellungen im Grund-Konfigurations-Modul sind weitestgehend selbst erklärend, aber wir gehen hier alle einzeln durch:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configuration/config_mailhive.png&w=175&h=323&zc=1&q=100 "Basic Configuration Settings")](http://www.mailbeez.de/images/doc/configuration/config_mailhive.png "Basic Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Generelle Einstellungen

**Modul aktivieren?**  
 Diese Einstellung aktiviert bzw. deaktiviert MailBeez. Die Einstellung “True” bedeutet, dass MailBeez aktiv und einsatzbereit ist!

Nach der Installation befindet sich MailBeez im Simulations-Modus, es ist also sicher mit MailBeez zu spielen und alles zu testen, ohne dass Kunden Emails erhalten werden.

### Sicherheits-Einstellungen

**Sicherheits-Schlüssel**  
 Diese Einstellung schützt MailBeez vor unbefugter Ausführung. Lassen Sie diesen Wert wie er ist, bis Sie eventuell Bedarf bekommen, den Schlüssel zu verändern.

### Kompatibilitäts-Einstellungen

**Popup Fenster**  
 Bitte nur ändern, falls die AJAX (CeeBox) Popups nicht richtig öffnen – z.B. bei der Vorschau der Vorlagen

### Weitergehende Einstellungen

**Versions-Check Erinnerung**  
 Bestimmen Sie, ob Sie MailBeez automatisch an die Versions-Prüfung vom MailBeez Grundsystem und den Modulen erinnern soll.

**Early Check” aktivieren**  
 Enabling “Early Check” adds an SQL query on a per item, per module basis.

Falls vom Modul verwendet, kann der “Early Check” aktiviert oder deaktiviert werden.  
 “Early Check” entfernt schon beim Generieren der Sende-Liste Empfänger, welche bereits eine Email erhalten haben.

## Simulations-Einstellungen

Die Simulations-Konfiguration erlaubt es, verschieden Aspekte der Simulation zu konfigurieren:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configuration/config_simulation.png&w=175&h=295&zc=1&q=100 "Simulation Settings")](http://www.mailbeez.de/images/doc/configuration/config_simulation.png "Simulation Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Optionen zur Simulations-Kontrolle

**Neu-Start Button**  
 Mit einem Klick auf diesen Button werden alle protokollierten Simulations-Daten gelöscht.

**Betriebsart**  
 Zum Testen bitte “Simulation” wählen, in “Produktion” werden Emails an Kunden verschickt! Wenn Sie also nach ausgiebigen Testen mit den Ergebnissen der generierten Emails zufrieden sind, können Sie das MailBeez System sicher in Produktion nehmen.

**Simulations-Protokollierung**  
 Im Simulations Modus den Versand protokollieren? Zum Neu-Start von Simulationen das Simulations-Protokoll löschen.

MailBeez protokolliert, welche Email and welchen Kunden gesendet wurde, um sicherzustellen, dass Kunden keine doppelten (mehrfachen) Emails erhalten. Mit dieser Einstellung können Sie diese Protokollieren im Simulationsmodus konfigurieren.

### Optionen zu Simulations-Emails

**Email-Adresse für Simulationen**  
 An welche Email-Adresse sollen die Simulations-Emails geschickt werden? Alle generierten Emails werden an diese Email-Adresse versendet.

**Kopie-Versand bei Simulation**  
 Kopien an die konfigurierte Kopie-Adresse (unter Grund-Einstellungen) auch im Simulations Modus verschicken?

Wenn die Email-Adresse für “Kopie-An” und “Email-Adresse für Simulationen” identisch sind, werden Sie 2 Kopien jeder Simulation erhalten – es sei denn, Sie setzen diese Einstellung auf “False”.



## Weitere Schritte

Fast geschafft! Der letzte Schritt vor dem Testen ist die Konfiguration des zu testenden Modules. Dies ist schnell und einfach erledigt:

[Weiter zu den MailBeez Module Konfigurations Tutorials](/dokumentation/tutorials/mailbeez-tutorials/)

Wenn Sie noch kein zusätzliches Modul installiert haben, können Sie einfach mit dem bereits vorhanden Modul für “Geburtstags-Glückwünsche” beginnen – dieses Modul muss aber auch erst [installiert und konfiguriert werden](/dokumentation/tutorials/mailbeez-tutorials/geburstags-glueckwuensche-konfiguration-tutorial/) .

Wenn Sie bevorzugen, mit der Konfiguration des MailBeez Systems fortzufahren, bevor Sie ein Modul einrichten wollen, lesen Sie Bitte das Tutorial [MailBeez Konfiguration ausführlich](/dokumentation/tutorials/mailbeez-konfiguration-ausfuehrlich/). Dies wird nur ein paar Minuten in Anspruch nehmen.
