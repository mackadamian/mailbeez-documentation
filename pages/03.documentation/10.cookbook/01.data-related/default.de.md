---
# http://learn.getgrav.org/content/headers
title: Daten Grundlagen
#menu: Beez-O-Graph
slug: daten-grundlagen
date: 17-02-2016
published: true
publish_date: 17-02-2016
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
--------------

[TOC]


## Email-Adressen eines alten Kundenstammes prüfen

### Problem
In einem 10 Jahre alten Shop ist die Wahrscheinlichkeit gross, dass die Email-Adressen von Alt-Kunden ungültig sind (Postfach wurden gelöscht, nimmt keine Emails mehr an o.ä). Daher soll geprüft werden, welche Email-Adressen noch gültig sind und welche als ungültig markiert werden sollen.

### Lösung

Es wird eine Info-Email an alle Kunden versendet. Ungültige Email-Adressen werden "bouncen" (es kommt eine Rückläufer-Email). Diese Information wird dann genutzt, um die betroffenen Email-Adressen im MailBeez System als ungültig zu markieren und von weiteren Emails-Aktionen auszuschliessen.

1. MailBeez Tarif mit [Newsletter Profi](/dokumentation/mailbeez/newsletter) Modul buchen

1. Im MailBeez [Email-System](/dokumentation/configbeez/config_email_engine) den Versand über Newsletter2Go konfigurieren (ggf. an dieser Stelle bei Newsletter2Go registrieren) und sicherstellen, dass genügend Email-Volumen vorhanden ist (ggf. kostenpflichtig aufladen)

1. Im [Newsletter Profi](/dokumentation/mailbeez/newsletter) Modul eine neue Liste "Alle Kunden auch ohne Abo" anlegen und in der Segmentierung konfigurieren, für welche Länder der Newsletter-Abo check ignoriert werden soll.

1. Im [Newsletter Profi](/dokumentation/mailbeez/newsletter) Modul eine neue Kampagne mit Liste "Alle Kunden auch ohne Abo" und darin einen neuen Newsletter anlegen. Als Text z.B. folgendes wählen: 

 > Um unseren Kundenservice zu verbessern, möchten wir gerne sicherstellen, dass Ihre Email-Adresse noch gültig ist. 
 > Falls Sie weiterhin Informationen von unser erhalten wollen, brauchen Sie weiter nichts zu unternehmen.
 >  
 > Andernfalls nutzen Sie bitten den “keine weiteren Emails” Link unten in dieser Email
 
1. Den Newsletter aktivieren und versenden.
 
Dank der Integration mit Newsletter2Go werden alle ungültigen Email-Adressen an das MailBeez System zurückgemeldet. Dieser Vorgang kann einige Tage dauern und kann im Beez-O-Graph mit Klick auf "bounces" nachvollzogen werden.

>>>>>Beim Versand von Massen-Emails erhöhen Rückläufer Emails das **Risiko**, dass der versendende Email-Server als **Spam-Versender** markiert wird und auf diversen Blacklisten landet. Daher sollten Sie für diese Aktion niemals Ihren eigenen Email-Server verwenden, sondern auf **zertifizierte Profi-Versendesysteme** wie Newsletter2Go zurückgreifen.