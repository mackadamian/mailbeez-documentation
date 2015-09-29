---
# http://learn.getgrav.org/content/headers
title: Shopauskunft Integration Suite
slug: config_shopauskunft_integration
# menu: Shopauskunft Integration Suite
date: 08-02-2012
published: true
publish_date: 08-02-2012
# unpublish_date: 08-02-2012
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
    code: 'config_shopauskunft_integration'
    category: [configbeez]
    compatiblity: [comp_osc,comp_cre,comp_digi,comp_zencart,comp_xtc,comp_gambio]
    thumbnail: 'http://www.mailbeez.com/wp-content/uploads/downloads/thumbnails/2012/02/icon_64.png'
    pro: 'pro'
    cert: 'true'
    price: '159 EUR'
    title_en: 'Shopauskunft Integration Suite'
    teaser_en: 'Integrate your valuable Ratings in MailBeez Campaigs and your Storefront (SEO)'
    title_de: 'Shopauskunft Integration Suite'
    teaser_de: 'Integrieren Sie Ihre wertvollen Bewertungen in MailBeez Kampagnen und den Shop (SEO)'
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

Entwickelt in enger Zusammenarbeit mit Shopauskunft.

[![](http://www.shopauskunft.de/res/sa_siegel_rand_180x_20b_586.jpg "Shopauskunft")](http://www.shopauskunft.de)**Händler mit entsprechendem Shopauskunft Enterprise-Vertrag können jetzt die wertvollen Bewertungen noch wirksamer im Onlineshop und sogar in MailBeez Email Kampagnen einsetzen.**

Wie vielen Online Händler haben Sie sich für Shopauskunft entschieden, um neuen und auch bestehenden Kunden Sicherheit und Vertrauen zu demonstrieren.

Mit der MailBeez Shopauskunft Integration Suite haben Sie jetzt mehr Flexibilität um positive Bewertungen besonders wirkungsvoll im Shop und sogar in von MailBeez generierten Email zu platzieren.

Basierend auf 100% anpassbaren Vorlagen können Sie z.B. 5-Sterne Bewertungen an besonders kritischen Stellen einsetzten, z.B. auf der Seite zur Kontoeröffnung oder auch beim Checkout. Hier hilft eine zufällige, positive Bewertung letzte Zweifel aus den Weg zu räumen.

Da die Bewertungen direkt in das HTML des Shops eingefügt werden, haben diesen einen positiven SEO Effekt – alle Bewertungen können somit von Suchmaschinen erfasst werden.

Durch die nahtlose Integration mit den MailBeez Email Kampagnen können Sie auf einfachste Weise z.B. in Emails zur [Kunden Rückgewinnung](/dokumentation/mailbeez/winback_advanced/ "Winback Advanced") oder auch beim [Kontakt von Kunden ohne Bestellung](/dokumentation/mailbeez/nopurchase_advanced/ "No Purchase Advanced") Ihre positive Bewertungen herausstellen und somit das Kaufverhalten positiv beeinflussen.

Die wichtigsten Funktionen im Überblick:

- Caching des Shopauskunft Bewertungs Feed für schnelle Ladezeiten
- Vorlagenbasierte Darstellung der Bewertungen
- Unbeschränkte Anzahl von Vorlagen zur Integration an verschieden Stellen, eine Vorlage für Email Integration.
- Auswahl der anzuzeigenden Bewertungen, z.B. “Mindestens 4 Sterne”
- Zufällige oder chronologische Auflistung der Bewertungen
- Einfachste “Drop-In” installation
- Einfachster Funktionsaufruf für die Einbindung der Ausgabe in den Onlineshop

und natürlich:

- Handhabung der Zusatzdaten des Shopauskunft Bewertungs Feeds – zeitraubende Anpassungen entfallen damit

### Anwendung:

Modul installieren und Konfigurieren – den API Feed konfigurieren wie im Adminbereich des Moduls beschrieben.

Mit der integrierten Test-Funktion kann der API Feed komfortabel getestet werden.

### Integration der Bewertungen in den Shop:

**osCommerce, ZenCart, CRE Loaded**

**** Um z.B. die Shopauskunft Bewertungen in der “Kontakt” Seite des Shopsystems einzubinden, bitte folgenden Code in die seite “contact\_us.php” einfügen:

> //include class
>     require_once(DIR_FS_CATALOG . 'mailhive/configbeez/config_shopauskunft_integration/classes/shopauskunft_integration.php');
>     // create new instance
>     $feed = new shopauskunft_integration();
>     // generate output (template, number of ratings, min stars, shuffle)
>     echo $feed->output_feed('feed_reviewpage.tpl', 7, 4, 'True');

Die mitgelieferte DIV/CSS basierende Vorlagee “rss\_reviewpage.tpl” lieferte folgende Ausgabe:

Mit dem Anlegen und Anpassen verschiedener eigener Vorlagen, z.B. “feed\_shoppingcart.tpl” für eine zufällige Bewertunge im Einkaufswagen – können die Shopauskunft Bewertungen sehr flexibel eingebunden werden.

**xt:Commerce, xtc-modified, Gambio GX**

Um z.B. die Shopauskunft Bewertungen in beliebigen Stellen im Shop-Frontend darstellen zu können, bitte folgende Schritte durchführen:

Datei

> templates//source/boxes.php

z.B. ganz am Ende vor dem ?> folgendes einfügen:

> // MailBeez Shopauskunft Integration Suite
>     require_once(DIR_FS_CATALOG . 'mailhive/configbeez/config_shopauskunft_integration/classes/shopauskunft_integration.php');
>     // create new instance
>     $feed = new shopauskunft_integration();
>     
>     // generate output (template, number of ratings, min stars, shuffle)
>     $smarty->assign('sabox_reviewpage', $feed->output_feed('feed_reviewpage.tpl', 25, 4, 'False') );
>     $smarty->assign('sabox_single', $feed->output_feed('feed_reviewpage.tpl', 1, 4, 'True') );
>     // - MailBeez Shopauskunft Integration Suite

Hiermit werden die Template-Variablen

> {$sabox_reviewpage}
> 
>  
>     {$sabox_single}

angelegt und basierend auf der Vorlagen “feed\_reviewpage.tpl” mit formatierten Bewertungen gefüllt.

Um z.B. eine einzelne Bewertung auf der “Kontakt”-Seite darzustellen, folgende Änderung vornehmen:

Datei

> templates//module/contact\_us.html

füge z.B. am Ende ein:

> {$sabox_single}

Die mitgelieferte DIV/CSS basierende Vorlage “feed\_reviewpage.tpl” lieferte folgende Ausgabe:

Mit dem Anlegen und Anpassen verschiedener eigener Vorlagen, z.B. “feed\_shoppingcart.tpl” für eine zufällige Bewertung im Einkaufswagen – können die Shopauskunft Bewertungen sehr flexibel eingebunden werden.

**Einbindung der Shopauskunft Bewertungen in MailBeez Kampagnen:**

Mit dem leichten Einfügen eines einfachen Platzhalters in MailBeez Vorlagen können Shopauskunft Bewertungen in alle oder ausgewählten von MailBeez generierten Emails angezeigt werden.
