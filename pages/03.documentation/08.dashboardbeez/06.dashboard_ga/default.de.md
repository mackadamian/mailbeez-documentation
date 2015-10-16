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




Als Bestandteil des MailBeez Grundsystemes erlaubt Ihnen der Der Google Analytics O'Pie schnell und einfach die vom Google Analytics erfassten Daten (Besucher, Umsatz) der MailBeez Emails einzusehen.

![](Screen_ga_dash_widget.png "Google Analytics-O-Pie")


>>>>>Um dieses Widget zu nutzen muss Google Analytics - gerne mit Ecommerce Tracking - im Shop installiert sein.

####Häufig gestellte Fragen 

**Warum unterscheiden sich die Google Analytics-Daten von MailBeez Analytics Data?**

Google Analytics kann nur Bestellungen verfolgen, die nach dem Klicken auf einen Link in einer von MailBeez generierten E-Mail getätigt wurde. Wenn zum Beispiel ein Kunde einen MailBeez Coupon auf seinem mobilen Gerät empfängt, aber später seine Bestellung auf seinem Computer durchführt und dabei den Rabatt-Code aus der Email abtippt, wird die Google Analytics Verbindung zum MailBeez Email verlieren.

Umgekehrt kann aber MailBeez alle Bestellungen mit generierten Coupons in MailBeez Analytics verfolgen, egal ob der Kunde den Link in der E-Mail klickt oder manuell in die Coupon-Code aus der E-Mail eintippt.

**Warum habe ich so wenigen Klicks in Google Analytics erfasst?** 

Einige Online-Shops haben kein Google Analytics-Tracking auf ihrer Start-Seite, nur auf Unterseiten. Wenn Ihre MailBeez E-Mails einen Link zu Start-Seite enthält, werden diese Besuche (und die daraus resultierenden Käufe), nicht von Google Analytics erfasst werden können.

 

## Das Google Analytics Dashboard Widget 

Um die Konfiguration zu erleichtern, folgen Sie bitte den folgenden Schritten:

>>>>Bitte Google Analytics im “alten” Layout verwenden

### Schritt 1: Erstellen Sie ein Google API Project 

1. Bitte gehen Sie zu : <https://code.google.com/apis/console/> und melden Sie sich ggf. an

2. Wenn Sie diese Seite zum ersten Mail nutzen, werden Sie ein “Create Project” Button finden. Diesen Anklicken:
![](Screen_create_project_button.png "Create Project Button")

4. Andernfalls werden Sie die Google API Services Console sehen. Wählen Sie “Services” aus dem linken Menü und aktivieren Sie die Analytics API aus der API Liste:
![](Screen_api_services_console.png "API Services Console - Services List")  
 **Hinweis:** Ggf. müssen Sie den Nutzungsbestimmungen zustimmen, bitte tun Sie dies.

7. Wählen Sie “API Access” aus dem linken Menü um zur Google API Access Console zu gelangen:
![](Screen_api_access_console1.png "API Access Console - Create Client ID")

9. Klicken Sie auf “Create an OAuth 2.0 client ID” Button um den “Create Client ID” Dialog zu öffnen:
![](Screen_create_client_id_popup1.png "Create Client ID - Step 1")

11. Im Feld “Product name” geben Sie bitte “MailBeez Application” (ohne Anführungszeichen) ein

12. Prüfen Sie das “Google Account” Feld. Hier sollten Sie Ihre Gmail Adresse finden.

13. Weiter mit dem “Next” Button:
![](Screen_create_client_id_popup2.png "Create Client ID - Step 2")

15. Wählen sie “Web application”. Geben Sie Ihre Shop-Domain ein.

16. Klicken Sie auf “More Options”
![](Screen_create_client_id_popup3.png "Create Client ID - Step 3")

18. Ändern Sie die Angabe für Authorized Redirect URIs – ersetzen sie “https://www.example.com/oauth2callback” mit der Angabe aus dem MailBeez Google Analytics Dashboard Widget

19. Klicken Sie auf “Create client ID”

20. Die API Einrichtung ist somit abgeschlossen und die Daten können in das MailBeez Google Analytics Dashboard Widget übernommen werden:
![](Screen_api_access_console2.png "API Access Console - Setup Complete")

22. Um diesen Schritt abzuschliessen, benötigen Sie die Client ID und das Client Secret von diesem Dialog:

### Schritt 2: Konfiguration des Dashboard Widgets

1. Navigieren Sie zum Google Analytics Dashboard Widget auf Ihrem MailBeez Dashboard:
![](Screen_ga_dash_config1.png "Google Analytics Dashboard Widget")

3. Geben Sie die Client ID und das Client Secret aus der Google API Console ein & und klicken Sie den “bestätigen” Button

4. Click the “Connect” button to connect your widget to your Google account:
![](Screen_ga_dash_config2.png "Connect to Google")

6. Wenn Sie nicht in bei Google angemeldet sind, werden Sie den Google Login Screen sehen. Melden Sie sich an, um zum Google Authentication Dialog zu gelangen.

7. Wenn Sie bei Google angemeldet sind, werden Sie direkt zum Google Authentication gelangen:
![](Screen_ga_authentication.png "Google Analytics Authentication Screen")

9. Klicken Sie auf “Zugriff erlauben” und Sie kommen zurück zum MailBeez Dashboard, wo Sie jetzt eine Liste der Google Profile sehen. Bitte wählen Sie das passende:
![](Screen_ga_dash_config3.png "Your Google Account Profiles")

11. Nach der Auswahl des Profils, werden Sie den Google Analytics-O-Pie sehen:
![](Screen_ga_dash_widget.png "Google Analytics-O-Pie")


Alternativ können Sie zur Konfiguriation des Widgets auch auf den “konfigurieren” Link unter dem Widget klicken, allerdings sollten Sie dort die Daten nur in Ausnahmefällen bearbeiten.
