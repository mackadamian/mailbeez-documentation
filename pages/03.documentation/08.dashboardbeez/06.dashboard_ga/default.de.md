---
# http://learn.getgrav.org/content/headers
title: Der Google Analytics O'Pie
slug: dashboard_ga
# menu: Der Google Analytics O'Pie
date: 07-05-2012
published: true
publish_date: 07-05-2012
# unpublish_date: 07-05-2012
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

####Häufig gestellte Fragen 

**Warum unterscheiden sich die Google Analytics-Daten von MailBeez Analytics Data?**

Google Analytics kann nur Bestellungen verfolgen, die nach dem Klicken auf einen Link in einer von MailBeez generierten E-Mail getätigt wurde. Wenn zum Beispiel ein Kunde einen MailBeez Coupon auf seinem mobilen Gerät empfängt, aber später seine Bestellung auf seinem Computer durchführt und dabei den Rabatt-Code aus der Email abtippt, wird die Google Analytics Verbindung zum MailBeez Email verlieren.

Umgekehrt kann aber MailBeez alle Bestellungen mit generierten Coupons in MailBeez Analytics verfolgen, egal ob der Kunde den Link in der E-Mail klickt oder manuell in die Coupon-Code aus der E-Mail eintippt.

**Warum habe ich so wenigen Klicks in Google Analytics erfasst?** 

Einige Online-Shops haben keine Google Analytics-Tracking auf ihrer Start-Seite, nur auf Unterseiten. Wenn Ihre MailBeez E-Mails einen Link zu Start-Seite enthält,  
 werden diese Besuche (und die daraus resultierenden Käufe), nicht von Google Analytics erfasst werden.

 

## Das Google Analytics Dashboard Widget 

Aufgrund von Änderungen an der Google Analytics API, hat sich auch die Konfiguration des MailBeez Google Analytics Dashboard Widgets verändert. Es gibt jetzt einen neuen Ablauf, um dem MailBeez Dashboard Widget Zugriff auf die Google Analytics Daten zu gewährleisten.

Hierzu haben wir eine Schritt-für-Schritt-Anleitung für Sie erstellt, um die Konfiguration zu erleichtern:

**WICHTIG:** Bitte Google Analytics im “alten” Layout verwenden

###  Schritt 1: Erstellen Sie ein Google API Project 

1. Bitte gehen Sie zu : <https://code.google.com/apis/console/> und melden Sie sich ggf. an
2. Wenn Sie diese Seite zum ersten Mail nutzen, werden Sie ein “Create Project” Button finden. Diesen Anklicken:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/create_project_button.png&w=270&h=252&zc=1&q=100 "Create Project Button")](http://www.mailbeez.de/images/doc/ga_dash_config/create_project_button.png "Create Project Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Andernfalls werden Sie die Google API Services Console sehen. Wählen Sie “Services” aus dem linken Menü und aktivieren Sie die Analytics API aus der API Liste:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/api_services_console.png&w=270&h=145&zc=1&q=100 "API Services Console - Services List")](http://www.mailbeez.de/images/doc/ga_dash_config/api_services_console.png "API Services Console - Services List")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Hinweis:**Ggf. müssen Sie den Nutzungsbestimmungen zustimmen, bitte tun Sie dies.

7. Wählen Sie “API Access” aus dem linken Menü um zur Google API Access Console zu gelangen:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/api_access_console1.png&w=270&h=140&zc=1&q=100 "API Access Console - Create Client ID")](http://www.mailbeez.de/images/doc/ga_dash_config/api_access_console1.png "API Access Console - Create Client ID")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

9. Klicken Sie auf “Create an OAuth 2.0 client ID” Button um den “Create Client ID” Dialog zu öffnen:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/create_client_id_popup1.png&w=270&h=160&zc=1&q=100 "Create Client ID - Step 1")](http://www.mailbeez.de/images/doc/ga_dash_config/create_client_id_popup1.png "Create Client ID - Step 1")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

11. Im Feld “Product name” geben Sie bitte “MailBeez Application” (ohne Anführungszeichen) ein
12. Prüfen Sie das “Google Account” Feld. Hier sollten Sie Ihre Gmail Adresse finden.
13. Weiter mit dem “Next” Button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/create_client_id_popup2.png&w=270&h=181&zc=1&q=100 "Create Client ID - Step 2")](http://www.mailbeez.de/images/doc/ga_dash_config/create_client_id_popup2.png "Create Client ID - Step 2")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

15. Wählen sie “Web application”. Geben Sie Ihre Shop-Domain ein.
16. Klicken Sie auf “More Options”
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/create_client_id_popup3.png&w=270&h=202&zc=1&q=100 "Create Client ID - Step 3")](http://www.mailbeez.de/images/doc/ga_dash_config/create_client_id_popup3.png "Create Client ID - Step 3")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

18. Ändern Sie die Angabe für Authorized Redirect URIs – ersetzen sie “https://www.example.com/oauth2callback” mit der Angabe aus dem MailBeez Google Analytics Dashboard Widget
19. Klicken Sie auf “Create client ID”
20. Die API Einrichtung ist somit abgeschlossen und die Daten können in das MailBeez Google Analytics Dashboard Widget übernommen werden:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/api_access_console2.png&w=270&h=212&zc=1&q=100 "API Access Console - Setup Complete")](http://www.mailbeez.de/images/doc/ga_dash_config/api_access_console2.png "API Access Console - Setup Complete")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

22. Um diesen Schritt abzuschliessen, benötigen Sie die Client ID und das Client Secret von diesem Dialog:

### Step 2: Konfiguration des Dashboard Widgets

1. Navigieren Sie zum Google Analytics Dashboard Widget auf Ihrem MailBeez Dashboard:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/ga_dash_config1.png&w=270&h=96&zc=1&q=100 "Google Analytics Dashboard Widget")](http://www.mailbeez.de/images/doc/ga_dash_config/ga_dash_config1.png "Google Analytics Dashboard Widget")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Geben Sie die Client ID und das Client Secret aus der Google API Console ein & und klicken Sie den “bestätigen” Button
4. Click the “Connect” button to connect your widget to your Google account:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/ga_dash_config2.png&w=270&h=95&zc=1&q=100 "Connect to Google")](http://www.mailbeez.de/images/doc/ga_dash_config/ga_dash_config2.png "Connect to Google")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

6. Wenn Sie nicht in bei Google angemeldet sind, werden Sie den Google Login Screen sehen. Melden Sie sich an, um zum Google Authentication Dialog zu gelangen.
7. Wenn Sie bei Google angemeldet sind, werden Sie direkt zum Google Authentication gelangen:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/ga_authentication.png&w=270&h=79&zc=1&q=100 "Google Analytics Authentication Screen")](http://www.mailbeez.de/images/doc/ga_dash_config/ga_authentication.png "Google Analytics Authentication Screen")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

9. Klicken Sie auf “Zugriff erlauben” und Sie kommen zurück zum MailBeez Dashboard, wo Sie jetzt eine Liste der Google Profile sehen. Bitte wählen Sie das passende:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/ga_dash_config3.png&w=270&h=94&zc=1&q=100 "Your Google Account Profiles")](http://www.mailbeez.de/images/doc/ga_dash_config/ga_dash_config3.png "Your Google Account Profiles")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

11. Nach der Auswahl des Profils, werden Sie den Google Analytics-O-Pie sehen:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.de/images/doc/ga_dash_config/ga_dash_widget.png&w=270&h=116&zc=1&q=100 "Google Analytics-O-Pie")](http://www.mailbeez.de/images/doc/ga_dash_config/ga_dash_widget.png "Google Analytics-O-Pie")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


Alternativ können Sie zur Konfiguriation des Widgets auch auf den “konfigurieren” Link unter dem Widget klicken.
