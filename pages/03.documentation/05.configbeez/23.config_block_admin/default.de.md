---
# http://learn.getgrav.org/content/headers
title: Erweitertes Opt-out mit Admin
slug: config_block_admin
# menu: Erweitertes Opt-out mit Admin
date: 18-10-2011
published: true
publish_date: 18-10-2011
# unpublish_date: 18-10-2011
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
module:
    code: 'config_block_admin'
    category: [configbeez]
    compatiblity: [comp_osc,comp_cre,comp_digi,comp_zencart,comp_xtc,comp_gambio]
    thumbnail: 'http://www.mailbeez.com/wp-content/uploads/downloads/thumbnails/2011/10/icon_325.png'
    pro: 'pro'
    cert: 'true'
    price: '99 EUR'
    title_en: 'Advanced Opt-Out with Admin'
    teaser_en: 'Block all modules and administer customers opt-out settings'
    title_de: 'Erweitertes Opt-out mit Admin'
    teaser_de: 'Alle Module blockieren und Opt-Out der Kunden administrieren'
    author: 'MailBeez.com'
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

**Früher oder später wird der Zeitpunkt kommen, an dem man gerne selbst bestimmen möchte, welche der Kunden eine von MailBeez generierte Email erhalten soll (oder eben nicht). Dann hilft dieses Modul schnell und einfach weiter.**

Dieses Modul erweitert die Opt-Out Funktion von MailBeez und bietet dem Administrator die Möglichkeit, “Opt-Outs” der Kunden manuel zu bearbeiten.

## Erweitertes Opt-Out

Die Erweiterung der Opt-Out Funktion umfasst:

**Opt-Out aller MailBeez Emails**

Mit der Vorlagen-Variable {$block\_all\_url} kann ein zusätzlicher Link in die Fusszeile der Hauptvorlage eingefügt werden, z.B. wie **fett** markiert

> [keine weiteren Emails dieser Art]({$block_url})  
>  |  
> **[generell keine weiteren Emails]({$block_all_url})**

**Opt-Out für bestimmte Module unterbinden**

Es gibt aber einige Module, welche Kunden nicht blockieren können sollen wie z.B. Zahlungserinnerungen, Hierzu kann per Mausklick eine Liste an Ausnahmen definiert werden.

Mit folgendem Code in der Fusszeile der Email Vorlage kann die Ausgabe der Opt-Out Links gesteuert werden. Natürlich sind die Opt-Out Links selbst auch inaktiv falls diese in der Email verbleiben sollen.

> <strong>{if $noblock}</strong>
>       Sie können diese Benachrichtigung nicht abbestellen
>     <strong>{else}</strong>
>     <a href="{$block_url}">keine weiteren Emails dieser Art</a>
>     |
>     <a href="{$block_all_url}">generell keine weiteren Emails</a>
>     <strong>{/if}</strong>

## Opt-Out Administration

Jede von MailBeez generierte Email stellt bereits einen Link “Keine weiteren Emails dieser Art” in der Fusszeile zur Verfügung. Hiermit können Kunden selbst entscheiden, ob Sie weitere Emails erhalten wollen oder nicht. Das “Kunden Opt-out Admin” Modul geht einen Schritt weiter und bietet die Möglichkeit manuell bestimmt Kunden für einzelne oder alle MailBeez Module zu blockieren.

Ebenso gibt es aber auch die Situation, dass Kunden versehentlich oder aus Neugierde den Link “Keine weiteren Emails dieser Art” anklicken, dann aber doch weitere Angebote erhalten möchten und den Shopbetreiber dies bezüglich kontaktieren. Mit einer schnellen Suche mit Kundennummer, Email Adresse oder Namen ist der Vorgang in wenigen Sekunden erledigt.



## Neu in Version 2.8: Massen-Verarbeitung

Haben Sie Email-Adressen aus anderen Mail-Programmen und möchten Sie die dazugehörigen Kunden in MailBeez blockieren? Mit dieser neuen Funktion ist es in wenigen Schritten erledigt

- Fügen Sie die zu verarbeitenden Email-Adressen in das Eingabe-Feld ein, je Zeile eine Email-Adresse
- Wählen Sie die zu blockierenden Module
- Die Email-Adressen werden automatisch verarbeitet und die dazugehörigen Kunden blockiert
V2.8
- opt-out importer

V2.75
- fixed a bug where in some occasions the check against "ALL" did not work

V2.7
- fixed a bug where in some occasions the check against "ALL" did not work

V2.6
- minor improvements

V2.5
- compatiblity MailBeez V2.7.2

V2.4
- compatibility with MailBeez V2.7
- minor bugfixes