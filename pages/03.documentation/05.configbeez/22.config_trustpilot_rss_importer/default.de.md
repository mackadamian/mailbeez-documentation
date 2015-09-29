---
# http://learn.getgrav.org/content/headers
title: Trustpilot Integration Suite
slug: config_trustpilot_rss_importer
# menu: Trustpilot Integration Suite
date: 03-05-2011
published: true
publish_date: 03-05-2011
# unpublish_date: 03-05-2011
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
    code: 'config_trustpilot_rss_importer'
    category: [configbeez]
    compatiblity: [comp_osc,comp_cre,comp_digi,comp_zencart,comp_xtc,comp_gambio]
    thumbnail: 'http://www.mailbeez.com/wp-content/uploads/downloads/thumbnails/2011/03/top_64.png'
    pro: 'pro'
    cert: 'true'
    price: '159 EUR'
    title_en: 'Trustpilot Integration Suite'
    teaser_en: 'Integrate your valuable Trustpilot Ratings in MailBeez Campaigs and your Storefront (SEO)'
    title_de: 'Trustpilot Integration Suite'
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

**Händler mit entsprechendem Trustpilot-Vertrag können jetzt die wertvollen Bewertungen noch wirksamer im Onlineshop und sogar in MailBeez Email Kampagnen einsetzen.**

Wie vielen Online Händler haben Sie sich für Trustpilot entschieden, um neuen und auch bestehenden Kunden Sicherheit und Vertrauen zu demonstrieren.

Mit der MailBeez Trustpilot Integration Suite haben Sie jetzt mehr Flexibilität um positive Bewertungen besonders wirkungsvoll im Shop und sogar in von MailBeez generierten Email zu platzieren.

Basierend auf 100% anpassbaren Vorlagen können Sie z.B. 5-Sterne Bewertungen an besonders kritischen Stellen einsetzten, z.B. auf der Seite zur Kontoeröffnung oder auch beim Checkout. Hier hilft eine zufällige, positive Bewertung letzte Zweifel aus den Weg zu räumen.

Da die Bewertungen direkt in das HTML des Shops eingefügt werden, haben diesen einen positiven SEO Effekt – alle Bewertungen können somit von Suchmaschinen erfasst werden.

Durch die nahtlose Integration mit den MailBeez Email Kampagnen können Sie auf einfachste Weise z.B. in Emails zur [Kunden Rückgewinnung](/documentation/mailbeez/winback_advanced/ "Winback Advanced") oder auch beim [Kontakt von Kunden ohne Bestellung](/documentation/mailbeez/nopurchase_advanced/ "No Purchase Advanced") Ihre positive Bewertungen herausstellen und somit das Kaufverhalten positiv beeinflussen.

Die wichtigsten Funktionen im Überblick:

- Caching des Trustpilot Bewertunge Feed für schnelle Ladezeiten
- Vorlagenbasierte Darstellung der Bewertungen
- Unbeschränkte Anzahl von Vorlagen zur Integration an verschieden Stellen, eine Vorlage für Email Integration.
- Auswahl der anzuzeigenden Bewertungen, z.B. “Mindestens 4 Sterne”
- Zufällige oder chronologische Auflistung der Bewertungen
- Einfachste “Drop-In” installatoin
- Einfachster Funktionsaufruf für die Einbindung der Ausgabe in den Onlineshop

und natürlich:

- Handhabung der Inkompatibilitäten und Zusatzdaten des Trustpilot Bewertungs Feeds – zeitraubende Anpassungen entfallen damit

### Anwendung:

Modul installieren und Konfigurieren – den RSS Feed konfigurieren wie im Adminbereich des Moduls beschrieben.

Mit der integrierten Test-Funktion kann der RSS Feed komfortabel getestet werden.

### Integration der Bewertungen in den Shop:

**osCommerce, ZenCart, CRE Loaded**  
 Um z.B. die Trustpilot Bewertungen in der “Kontakt” Seite des Shopsystems einzubinden, bitte folgenden Code in die seite “contact\_us.php” einfügen:

> //include class
>     require_once(DIR_FS_CATALOG . 'mailhive/configbeez/config_trustpilot_rss_importer/classes/trustpilot_import_rss.php');
>     // create new instance
>     $rss = new trustpilot_import_rss();
>     // generate output (template, number of ratings, min stars, shuffle)
>     echo $rss->output_rss('rss_reviewpage.tpl', 7, 4, 'True');

Die mitgelieferte DIV/CSS basierende Vorlagee “rss\_reviewpage.tpl” liefert folgende Ausgabe:

[![](http://www.mailbeez.com/wp-content/uploads/2011/05/default_reviewpage_template-300x262.png "default_reviewpage_template")](http://www.mailbeez.com/wp-content/uploads/2011/05/default_reviewpage_template.png)Standard Vorlage für Trustpilot Bewertungen

 

 

**xt:Commerce, xtc-modified, Gambio GX**  
 Um z.B. die Trustpilot Bewertungen in beliebigen Stellen im Shop-Frontend darstellen zu können, bitte folgende Schritte durchführen:

Datei

> templates/<dein template>/source/boxes.php

z.B. ganz am Ende vor dem ?> folgendes einfügen:

> // MailBeez Trustpiloshops Integration Suite
>     require_once(DIR_FS_CATALOG . 'mailhive/configbeez/config_trustpilot_rss_importer/classes/trustpilot_import_rss.php');
>     // create new instance
>     $rss = new trustpilot_import_rss();
>     
>     // generate output (template, number of ratings, min stars, shuffle)
>     $smarty->assign('tpbox_reviewpage', $rss->output_rss('rss_reviewpage.tpl', 25, 4, 'False') );
>     $smarty->assign('tpbox_single', $rss->output_rss('rss_reviewpage.tpl', 1, 4, 'True') );
>     // - MailBeez Trustpiloshops Integration Suite

 

Hiermit werden die Template-Variablen

> {$tpbox_reviewpage}
> 
>  
>     {$tpbox_single}

angelegt und basierend auf der Vorlagen “rss\_reviewpage.tpl” mit formatierten Bewertungen gefüllt.

Um z.B. eine einzelne Bewertung auf der “Kontakt”-Seite darzustellen, folgende Änderung vornehmen:

Datei

> templates/<dein template>/module/contact\_us.html

füge z.B. am Ende ein:

> {$tpbox_single}

 

[![](http://www.mailbeez.com/wp-content/uploads/2011/05/trustpilot_rss_contact_us_xtcm-250x114.png "trustpilot_rss_contact_us_xtcm")](http://www.mailbeez.com/wp-content/uploads/2011/05/trustpilot_rss_contact_us_xtcm.png)Zufälliges Trustpilot Rating

 

 

Mit dem Anlegen und Anpassen verschiedener eigener Vorlagen, z.B. “rss\_shoppingcart.tpl” für eine zufällige Bewertunge im Einkaufwagen – können die Trustpilot Bewertungen sehr flexibel eingebunden werden.

**Einbindung der Trustpilot Bewertungen in MailBeez Kampagnen:**  
 Mit dem leichten Einfügen eines einfachen Platzhalters in MailBeez Vorlagen können Trustpilot Bewertungen in alle oder ausgewählten von MailBeez generierten Emails angezeigt werden. Mehr hierzu auf der Seite zum Hilfsmodule [Trustpilot Bewertungen in Emails](/documentation/filterbeez/filter_add_trustpilot_rss/?lang=de "Add Trustpilot Ratings").

[![](http://www.mailbeez.com/wp-content/uploads/2011/05/default_email_template-300x289.png "default_email_template")](http://www.mailbeez.com/wp-content/uploads/2011/05/default_email_template.png)Standard Vorlage für Email Integration

 

 

- - - - - -

Ein Bespiel zur Einbindung:

## Showcase: Alwaysriding

[![](http://www.mailbeez.com/wp-content/uploads/2011/05/trustpilot_reviewpage-300x255.png "trustpilot_reviewpage")](http://www.mailbeez.com/wp-content/uploads/2011/05/trustpilot_reviewpage.png)Seite mit Bewertungen – custom design

 

Wie wohl kaum ein anderer versteht Alwaysriding.co.uk die Wichtigkeit einer vertrauensvollen Kundenbeziehung – die Kunden danken dies mit sehr positiven Bewertungen auf Trustpilot.

 

Diese Bewertungen sind sehr wertvoll, da sie die hohe Qualität des Anbieters und die hohe Kundenzufriedenheit widerspiegeln – da diese Bewertungen auf dem unabhängigen Trustpilot system verwaltet werden, haben Sie eine hohe Glaubwürdigkeit.

Die Trustpilot Integration Suite von MailBeez erlaubt Alwaysriding diese Bewertunge bestmöglich zur Gewinnung von Neukunden und/oder widergewinnung von Altkunden zu verwenden..

[![](http://www.mailbeez.com/wp-content/uploads/2011/05/trustpilot_cart-300x255.png "trustpilot_cart")](http://www.mailbeez.com/wp-content/uploads/2011/05/trustpilot_cart.png)Einkaufswagen mit Bewertungen – custom design

 

Mit nur geringen Anpassungen am Shop hat Alwaysriding jetzt ein System implementiert, welches automatisch Trustpilot bewertungen importiert und anzeigt.

Der Einkaufswagen ist eine sehr geeignete Stelle, um Kunden von Ihren positiven Erfahrungen berichten zu lassen.

 

Die neuesten Bewertungen sind auf einer eigenständigen Seite aufgelistet – mit Verlinkung zu Trustpilot.

Aber der Shop ist natürlich nicht die einzige Stelle, an der Trustpilot Bewertungen die Kaufentscheidung positiv beeinflussen.

[![](http://www.mailbeez.com/wp-content/uploads/2011/05/trustpilot_mailbeez-165x300.png "trustpilot_mailbeez")](http://www.mailbeez.com/wp-content/uploads/2011/05/trustpilot_mailbeez.png)Einbindung in MailBeez Kampagnen – custom design

 

Mit Hilfe der Trustpilot Integration Suite wird das beliebte und effektive Modul “Kunden ohne Kauf” (Nopurchase) mit positiven Kundenstimmen aufgewerten.

Dies passiert voll automatisch und kann mit einem einfachen Platzhalter eingebunden werden – natürlich in jedem MailBeez Modul und in jeder MailBeez Email Kampagne.
