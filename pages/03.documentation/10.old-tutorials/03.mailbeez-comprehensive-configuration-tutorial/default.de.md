---
# http://learn.getgrav.org/content/headers
title: MailBeez Konfiguration ausführlich
slug: mailbeez-konfiguration-ausfuehrlich
# menu: MailBeez Konfiguration ausführlich
date: 11-07-2012
published: true
publish_date: 11-07-2012
# unpublish_date: 11-07-2012
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

Die hier verwendeten Screenshots wurden mit ZenCart erstellt. Auf anderen Shop-System wird das Admin-Interface etwas anders aussehen, der Aufbau und die Bedienkonzepte sind aber einheitlich für alle Platformen – soweit nicht ausdrücklich auf Abweichungen hingewiesen wird.

## Los geht’s

Öffnen Sie MailBeez in Ihrer Shop-Administration und klicken Sie auf den “Konfiguration” Reiter. Sie werden dort eine Reihe von Konfigurations-Gruppen vorfinden:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/common_images/config_tab.png&w=270&h=134&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.de/images/doc/common_images/config_tab.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Jede Konfigurations-Gruppe besteht aus eine Reihe von Einstellungen, mit denen das MailBeez System an Ihre Anforderungen angepasst werden kann. In den meisten Fällen sollten die Grundeinstellungen schon passend sein.

In diesem Tutorial werden wir alle Konfigurations-Gruppen und die dazugehörigen Einstellungen durchgehen. Dies wird etwa 15-30 Minuten in Anspruch nehmen.

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

## Antispam Regeln

Die Einhaltung von Antispam Regeln kann hier konfiguriert werden

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configuration/config_spam_compliance.png&w=175&h=233&zc=1&q=100 "Spam Compliance Settings")](http://www.mailbeez.de/images/doc/configuration/config_spam_compliance.png "Spam Compliance Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Zustimmung der Kunden

**Newsletter Abo Check**  
 Entscheiden Sie, ob Sie ausschliesslich Kunden mit Newsletter Abo kontaktieren wollen.

Einige Module, z.B. Zahlungserinnerungen, werden diesen Check ignorieren.

Restriktive Einstellung: “True”

### Opt-Out Verhalten

**was passiert beim Klicken des Opt-Out Linkes?**  
 Jede MailBeez Email enthält einen Link “Keine weiteren Emails”. Standardmässig (Einstellung “Module”) wird nur das aktuelle Modul blockiert (z.B. “Bitte um Produktbewertungen”) während andere Module, z.B. Geburtstagsglückwünsche weiterhin versendet werden.

Die Einstellung “Global” bewirkt, dass die Abmeldung einer Art von Emails sich auf alle Emails auswirkt. Bei Bedarf können Sie den Opt-Out Link in der Email Vorlage entsprechend benennen.

Einige Module, wie z.B. “Zahlungserinnerung” werden diese Einstellungen ignorieren, da es sich um System-Emails handelt, die – genau wie die Bestellbestätigungs-Email – keine weitere Einwilligung des Kunden erfordert.

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

## Email System Einstellungen

Falls alles funktionert, brauchen diese Einstellungen nicht bearbeitet zu werden.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configuration/config_email_engine.png&w=149&h=396&zc=1&q=100 "Email Engine Settings")](http://www.mailbeez.de/images/doc/configuration/config_email_engine.png "Email Engine Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Email Vorlagen System wählen

**Übergehe das Zencart Email Vorlagen System**  
**Diese Einstellung existiert nur auf Zencart Installationen**  
 Es wird empfohlen, das MailBeez Vorlagen System zu nutzen, da dies volle Kontrolle über die Inhalte ermöglicht.  
**Double Dot Bugfix**  
 In seltenen Fällen wird der Punkt in Dateinamen verdoppelt, z.B. aus file.php wird file..php, image.png wird zu image..png. Sollten Sie dieses Problem beobachten, aktivieren Sie bitte diese Option.

### Email System einstellungen

**Wählen Sie das Email System**  
 Mit dieser Einstellung können Sie wählen, ob MailBeez die Email-Funktion des Shop-Systems verwendet oder den in MailBeez integrierten “PHPMailer”, welcher mit SMTP Email Accounts arbeitet.

Wenn Sie die [Email Rückfläufer-Verarbeitung](/dokumentation/configbeez/config_bouncehive_advanced/) einsetzen wollen, ist es zwingend erforderlich, dass PHPMailer Email System zu verwenden. Weitere Informationen hierzu finden Sie im [ MailBeez Email Rückfläufer-Verarbeitung Tutorial](/dokumentation/tutorials/configbeez-tutorials/-bounce-handling-configuration-tutorial/)

## Dashboard Konfiguration

Bestimmen Sie, wie das MailBeez Dashboard aussehen soll:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configuration/config_dash1.png&w=175&h=197&zc=1&q=100 "Dashboard Configuration Settings")](http://www.mailbeez.de/images/doc/configuration/config_dash1.png "Dashboard Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

## Ereignis Protokollierung

MailBeez protokolliert jede Ausführung des Systemes. Falls es Problem gibt, können Sie weitere Daten zur Fehlerlokalisierung protokollieren.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configuration/config_event_log.png&w=175&h=105&zc=1&q=100 "Event Log Settings")](http://www.mailbeez.de/images/doc/configuration/config_event_log.png "Event Log Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Das Ereignis-Protokoll finden Sie unter MailBeez > Berichte.

## MailHive Prozess Kontrolle

Bitte verändern Sie diese Einstellungen nicht – es sei denn, Sie wissen was Sie tun ![;-)](http://localhost/wordpress_mailbeez_EOL/wp-includes/images/smilies/icon_wink.gif)

## Google Analytics Integration

**Diese Einstellungen haben nur bei der Verwendung von Google Analytics eine Funktion**

### Google Analytics Einstellungen

**Google Analytics Integration**  
 Die Google Analytics Integration arbeitet global, d.h. für alle Module.  
**Google Analytics Umschreib-Modus**  
 Wählen Sie, wie Links in den Emails umgeschrieben werden, um das Klick-Tracking mit Google Analytics zu ermöglichen.

Wenn Sie einen bestimmten Link nicht umschreiben lassen wollen, fügen Sie einfach ein Leerzeichen vor und nach dem = bei href ein:

 
    <pre class="fancy_pre_box">
    Example: [html]<a href="http://www.mailbeez.com">Dieser Link wird umgeschrieben</a>[/html]
    Example: [html]<a href = "http://www.mailbeez.com">Dieser Link bleibt unverändert</a>[/html]


**Google Analytics URls in TXT Format umschreiben**  
 Entscheiden Sie, ob Sie die URLs im TXT Format der Emails umschreiben lassen wollen. Dadurch werden die URLs länger-

### Google Analytics Berichts-Einstellungen

**Google Analytics “Medium”**  
 Diese Kennung wird von Google Analytics als “Medium” verwendet und Sie können in Google Analytics hiernach selektieren.

**Google Analytics “Quelle”**  
 Diese Kennung wird von Google Analytics als “Medium” verwendet und Sie können in Google Analytics hiernach selektieren.

## MailBeez Analytics Einstellungen

### Warum?

Zunächst einige Worte, was MailBeez Analytics ist und wie es funktioniert. Mit MailBeez Analytics können Sie folgende Aktivitäten beobachten:

- Öffnen von Emails (Html Emails mit geladenen Bildern)
- Klicks auf Links
- Bestellungen, welche Klicks auf Links folgen

Das Öffnen von Emails wird mit Hilfe der folgenden Methoden erfasst:

- Wenn das Tracker-Bild geladen wird, wird dies als Öffnen der Email erfasst
- Wenn ein Link in einer Email angeklickt wird, wird dies als Öffnen der Email erfasst

Das Tracker-Bild nutzt einen hoch-optimieren Aufruf, um die Server-Belastung so gering wie möglich zu halten: Jedes Öffnen wird zunächst in ein Log-File protokolliert. Bei jeder Ausführung von Mailhive wird dann dieses Log-File eingelesen und danach gelöscht.

Öffnen und Klicks in “Kopie-an” Emails werden nicht erfasst, da dies separate Emails mit eigener Kennung sind. Dies verhindert, dass die Kopie-Emails die Statistik verfälschen.

### MailBeez Analytics installieren

Bitte prüfen Sie, ob das direkte Empfänger Tracking in Ihrer Region zulässig ist  
 Using direct user tracking can be against the law in your country. Sie sind selbst dafür verantwortlich, sich über die gesetzlichen Bestimmungen zu informieren und sind voll für die Nutzung des Empfängertrackings verantwortlich.

1. Öffnen Sie MailBeez > Konifguration
2. Klicken Sie auf die MailBeez Analytics Einstellungen:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configuration/config_mb_analytics1.png&w=175&h=191&zc=1&q=100 "MailBeez Analytics Activation")](http://www.mailbeez.de/images/doc/configuration/config_mb_analytics1.png "MailBeez Analytics Activation")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Klicken Sie auf den Button
2. Sie erhalten weitere Anweisungen im Popup
3. Kopieren Sie den Code und lassen Sie das Popup geöffnent
4. Bearbeiten Sie folgende Datei Ihres Shop-Systemes und fügen Sie dort den Code wie beschrieben ein:
 

    <pre class="fancy_pre_box"> Ihr_Shop/includes/application_top.php

Kehren Sie danach zu MailBeez zurück und klicken Sie auf “Empfängertracking aktivieren”.

### MailBeez Analytics konfigurieren

Die Standard-Einstellungen sind passend für die meisten Shops, nehmen Sie nur dann Veränderungen an den Einstellungen vor, wenn dies erforderlich ist.

## Template Engine

Mit dem “Clear” Button können Sie die vorgenerierten, kompilierten Email Vorlagen löschen. Dies kann erforderlich sein, wenn Änderungen an Email-Vorlagen scheinbar nicht übernommen werden.

## Weitere Einstellungen

Die weiteren Einstellungen sind optional und stehen nach der Installation von Premium-Modulen zur Verfügung: **[ MailBeez website.](http://www.mailbeez.de/download/)**

- BounceHive Rückläufer Verarbeitung
- Emailversand drosseln
- MailBeez automatisch ausführen
- Vorlagen Verwaltung

**[ BounceHive Rückläufer Verarbeitung](/dokumentation/configbeez/config_bouncehive_advanced/)**  
 Email Rückläufer (Bounces) generieren ungewünschte Arbeit für den Shop-Betreiber. Jeder Rückläufer muss gelesen werden und der Kunde mit der ungültigen Email-Adresse deaktiviert werden.  
 Zudem können Rückläufer das Risko als Spamversender eingestuft zu werden, erhöhen und auch zu Problemen mit dem Hoster führen.

Diese Modul automatisiert die Verarbeitung von Email Rückläufern. Diese Rückläufer werden eingelesen, analysiert und die dazugehörigen Email-Adressen markiert. Dadurch wird der weitere Versand von Emails an diese ungültigen Adresse unterbunden.

**[Emailversand drosseln](/dokumentation/mailbeez/filter_do_throttling_simple/)**  
 Dieses Modul erlaubt es, die Versandrate zu kontrollieren, um ggf. Limits des Hosters einzuhalten.

**[MailBeez automatisch ausführen](/dokumentation/configbeez/config_cron_simple/)**  
 Um die Ausführung von MailBeez zu automatisieren, gibt es folgende Möglichkeiten:

- Die Einrichtung eines Cronjobs
- Die Installation dieses Modules

Ohne eine dieser Möglichkeiten wird MailBeez nicht automatisiert arbeiten können, d.h. der Shopbetreiber muss täglich die Module manuell ausführen. Das Modul “MailBeez automatisch ausführen” ist schnell installiert und für viele Shopbetreiber die einfache Alternative.

**[Vorlagen Verwaltung](/dokumentation/configbeez/config_tmplmngr/)**  
 Mit Hilfe dieses Modules können MailBeez Nutzer schnell und einfach alle Email-Vorlagen direkt im MailBeez System bearbeiten. Somit entfällt das aufwändige Arbeite mit FTP Programmen und Text-Editoren.

**[Mouseflow](/dokumentation/configbeez/config_mouseflow/)**  
 Mouseflow ist ein Online-System, welches einfach und kostengünstig die Optimierung des Shops ermöglich. Mouseflow zeigt Ihnen, wie Besucher auf Ihren Seiten navigieren, wo es Probleme gibt und wo Verbesserungspotential vorliegt.



## Weitere Schritte

Fast geschafft! Nur noch ein Modul konfigurieren und schon kann der erste Test erfolgen.

Falls Sie noch keine weiteren Module installiert haben, können Sie sofort mit dem Geburtstags-Modul beginnen, welches in der MailBeez Grundinstallation vorhanden ist. Hier eine Anleitung zur [Konfiguration des Geburtstags-Modules](/dokumentation/tutorials/mailbeez-tutorials/geburstags-glueckwuensche-konfiguration-tutorial/).
