---
# http://learn.getgrav.org/content/headers
title: Newsletter
#menu: Beez-O-Graph
slug: newsletter-rezepte
published: true
template: tutorial
# theme: false
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: done
    category: [docs]
    tag: [pro]

---

[TOC]


## Gutschein für Registrierung zum Newsletter

>>>>>> **Hinweis:** Unter Einhaltung von bestimmten Ausnahmeregelungen dürfen Shopbetreiber Ihre Kunden auch ohne explizite Einwilligung per Email kontaktieren, lesen Sie mehr auf [Rechtssichere Email-Werbung ohne ausdrückliche Einwilligung](/uber/rechtssicher-email-werbung-ohne-ausdruckliche-einwilligung-senden)


### Problem

Sie möchten Ihren Kunden einen Gutschein zusenden, sobald diese sich für den Newsletter registrieren

### Lösung

Mit Hilfe des [Newsletter Profi Modules](/dokumentation/mailbeez/newsletter) können Sie automatisiert einen frei konfigurierbaren Gutschein an Ihre Kunden nach Registrierung zum Newsletter versenden.

Hierzu gehen Sie bitte wie folgt vor:

####Erstellen einer dynamischen Empfängerliste

1. Navigieren Sie zum MailBeez Newsletter Modul `MailBeez > MailBeez Module > Newsletter Profi`
1. Klicken Sie rechts im Abschnitt `Listen einrichten` auf den Button `Listen bearbeiten`
1. Erstellen Sie eine neue Liste mit Namen z.B. `Willkommens Gutschein` und wählen Sie als Quelle für die neue Liste `Shop Newsletter-Abos` aus - Liste speichern.
1. Wählen Sie die neu erstellte Liste an und klicken Sie rechts im Abschnitt `Segmentierung` auf `Segmentierung bearbeiten` - es öffnet sich ein Fenster
1. In den Segmentierungs-Einstellungen im Abschnitt `Kunde` bitte folgendes konfigurieren:
    - Kunde seit mindestens Tagen: 0
    - Kunde seit höchstens Tagen: 1 (oder einen höheren Wert, wenn Sie auch älteren Kunden einen Gutschein zusenden wollen)
![List](Screen_welcome_list.de.png?lightbox=true)
1. Segmentierung speichern
1. Mit Klick auf `Segmentierung testen` können Sie sehen, welche Empfänger gefunden werden. Klicken Sie auf die Namen, um den Kunden-Insight des Kunden zu öffnen.

Sie haben somit eine Liste erstellt, welche aktuelle Newsletter-Subscriber liefert.



####Erstellen eines Willkommens-Newsletters

>>>>> Bitte vorher einen Vorlagen-Gutschein mit den gewünschten Werten anlegen - nutzen Sie ggf. die entsprechende Tour unter `MailBeez > Tour` (1. Tab)

1. Navigieren Sie zum MailBeez Newsletter Modul `MailBeez > MailBeez Module > Newsletter Profi`
1. Klicken Sie rechts im Abschnitt `Erstellen und Bearbeiten Sie Ihre Kampagnen` auf den Button `Kampagnen bearbeiten`
1. Erstellen Sie eine neue Kampagne mit Namen z.B. `Willkommens Emails` und wählen Sie als Standard-Liste die zuvor neu erstellte Liste `Willkommens Gutschein` - Kampagne speichern
1. Wählen Sie die neu erstellte Kampagne an und klicken Sie rechts `Kampagnen-Emails bearbeiten`.
1. Erstellen Sie einen neuen Newsletter
1. Wählen Sie rechts den passende Vorlagen-Gutschein und speichern Sie
1. Konfigurieren Sie rechts als Aktiv bis Datum z.B. den 1.1.2099 (also setzen Sie den Newsletter dauer-aktiv) und speichern Sie
1. Gestalten Sie im Hauptbereich die Email mit Hilfe des Visuellen Editors, mit Klick auf das + Icon können Sie auch ein Inhalts-Element für die Darstellung des Gutscheines einfügen.
    - Falls Ihre Online-Shop in mehreren Sprachen verfügbar ist, gestalten Sie die Emails ebenfalls für die anderen Sprachen
1. Wenn Sie zufrieden mit der Gestaltung sind und die Test-Emails gut Aussehen, können Sie den neuen Newsletter oben rechts mit Klick auf `als versandfertig freigeben` aktiv schalten. 

![List](Screen_welcome_email.de.png?lightbox=true)


Herzlichen Glückwunsch! Sie haben jetzt eine Willkommens-Newsletter erstellt, der bei der nächsten Ausführung des Versendeprozesses an die passenden Empfänger versendet wird!
