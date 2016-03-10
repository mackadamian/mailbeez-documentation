---
# http://learn.getgrav.org/content/headers
title: Run MailBeez Automatically
slug: run-mailbeez-automatically-configuration-tutorial
# menu: Run MailBeez Automatically
date: 07-08-2012
published: true
publish_date: 07-08-2012
# unpublish_date: 07-08-2012
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

## Über dieses Modul

Mit diesem einfachen MailBeez Zusatzmodul können Sie sich die für viele komplizierte Einrichtung eines Cronjobs sparen, um den Versand von MailBeez zu automatisieren. Statt dessen wird der Traffic der Besucher im Online-Shop genutzt, um MailBeez zu automatisieren. Für Online-Händler, welche schnell und einfach MailBeez einsetzen wollen, ist dieses Modul sehr praktisch.

## Los geht’s

1. In den Adminbereich des Online-Shops einloggen
2. Zu MailBeez navigieren und den Tab “Konfiguration” anwählen

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/common_images/config_tab2.png&w=270&h=175&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.de/images/doc/common_images/config_tab2.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Finden Sie das Modul “MailBeez automatisch ausführen und dieses anklicken.
2. Klicken Sie den “Installieren” Button, um das Modul zu installieren  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configbeez/config_cron_simple/cron_simple_config1.png&w=175&h=179&zc=1&q=100 "Modul installieren")](http://www.mailbeez.de/images/doc/configbeez/config_cron_simple/cron_simple_config1.png "Modul installieren")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Jetzt wird die Konfiguration des Modules sichtbar:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configbeez/config_cron_simple/cron_simple_config2.png&w=175&h=313&zc=1&q=100 "Einstellungen")](http://www.mailbeez.de/images/doc/configbeez/config_cron_simple/cron_simple_config2.png "Einstellungen")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

## Das Modul konfigurieren

### Das Modul freischalten

Bitte das Zertifikat bereithalten.

1. Klicken Sie auf den “Bearbeiten” Button, der zur Eingabe des Zertifikates gehört
2. Kopieren Sie Ihr persönliches Zertifikat aus der Liefer-Email von Avangate in das Eingabefeld und klicken Sie auf “speichern”

Das Modul ist jetzt freigeschaltet und kann konfiguriert werden.

### Grundeinstellungen

Klicken Sie den oberen “Bearbeiten” Button

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/configbeez/config_cron_simple/cron_simple_config3.png&w=175&h=135&zc=1&q=100 "Run MailBeez Automatically General Settings")](http://www.mailbeez.de/images/doc/configbeez/config_cron_simple/cron_simple_config3.png "Run MailBeez Automatically General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Modul aktivieren**  
 Mit dieser Einstellung kann das Modul ein- und ausgeschaltet werden. Die Voreinstellung ist “True”, also das Modul ist eingeschaltet und wirdEmails an Kunden versenden. Setzen Sie die Einstellung auf “False”, um das Modul zu de-aktivieren

**Zeitraum zwischen den Ausführungen von MailBeez (Stunden)**

Mit dieser Einstellung können Sie bestimmen, wieviele Stunden zwischen den Ausführungen von MailBeez vergehen sollen. Die Standard-Einstellung ist 24, also MailBeez wird einmal täglich ausgeführt werden.

Wenn Sie mit der Konfiguration fertig sind, klicken Sie den “Speichern” Button. Die Konfiguration des Modules ist damit abgeschlossen!
