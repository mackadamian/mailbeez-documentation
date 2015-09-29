---
# http://learn.getgrav.org/content/headers
title: Responsive Vorlagen Verwaltung
slug: config_tmplmngr
routes:
    aliases:
        - /dokumentation/configbeez/config_tmplmngr
# menu: Responsive Vorlagen Verwaltung
date: 30-06-2011
published: true
publish_date: 30-06-2011
# unpublish_date: 30-06-2011
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
    code: 'config_tmplmngr'
    category: [configbeez]
    compatiblity: [comp_osc,comp_cre,comp_digi,comp_zencart,comp_xtc,comp_gambio]
    thumbnail: 'http://www.mailbeez.com/wp-content/uploads/downloads/thumbnails/2011/08/icon_321.png'
    pro: 'pro'
    cert: 'true'
    price: '159 EUR'
    title_en: 'Responsive Template Manager'
    teaser_en: 'edit your campaign templates from you MailBeez admin and send responsive Emails'
    title_de: 'Responsive Vorlagen-Verwaltung'
    teaser_de: 'Bearbeite die MailBeez Vorlagen direkt in der Admin und versende responsive Emails'
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

**neue Version 2.2 – mehr Informationen kommen in Kürze**

**erfordert MailBeez V2.8+**

Der Vorlagen Editor für MailBeez

## Vorlagen Manager

Mit diesem Plugin können die Vorlagen der MailBeez Module komfortable von der MailBeez Administration aus bearbeitet werden.

 
			#gallery-2 {
				margin: auto;
			}
			#gallery-2 .gallery-item {
				float: left;
				margin-top: 10px;
				text-align: center;
				width: 50%;
			}
			#gallery-2 img {
				border: 2px solid #cfcfcf;
			}
			#gallery-2 .gallery-caption {
				margin-left: 0;
			}
			/* see gallery_shortcode() in wp-includes/media.php */
		  [![logo](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2014/06/logo-100x24.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2014/06/logo.png "logo")   [![shopgate](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2012/01/shopgate-200x175.gif)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2012/01/shopgate.gif "shopgate")  [![logo_thehive](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/08/logo_thehive-200x45.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/08/logo_thehive.png "logo_thehive")   [![logo_thehive](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/08/logo_thehive1-200x44.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/08/logo_thehive1.png "logo_thehive")  [![logo_thehive](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/08/logo_thehive2-200x44.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/08/logo_thehive2.png "logo_thehive")   [![cert](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/09/cert.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/09/cert.png "cert")  [![notification_done](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2010/09/notification_done.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2010/09/notification_done.png "notification_done")   [![notification_error](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2010/09/notification_error.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2010/09/notification_error.png "notification_error")  [![notification_warning](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2010/09/notification_warning.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2010/09/notification_warning.png "notification_warning")   [![notification_error_big](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2010/09/notification_error_big.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2010/09/notification_error_big.png "notification_error_big")  [![zc_modules](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/01/zc_modules-199x105.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/01/zc_modules.png "zc_modules")   [![mailbeez_logo_4_400x100_trans](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/02/mailbeez_logo_4_400x100_trans-200x50.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/02/mailbeez_logo_4_400x100_trans.png "mailbeez_logo_4_400x100_trans")  [![info](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/05/info.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/05/info.png "info")   [![multilanguage](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/05/multilanguage.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/05/multilanguage.png "multilanguage")  [![payment_inadvance_dunning](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/06/payment_inadvance_dunning.png)](http://localhost/wordpress_mailbeez_EOL/wp-content/uploads/2011/06/payment_inadvance_dunning.png "payment_inadvance_dunning") 

Nach einer einfachen Installation – lediglich die neuen Dateien an die vorgesehen Stelle kopieren – steht sofort ein “Bearbeiten” Button in allen bearbeitbaren MailBeez Modulen zur Verfügung und auch die gemeinsame Hauptvorlage kann bearbeitet werden.

[![](http://www.mailbeez.com/wp-content/uploads/2011/03/edit_button.png "edit_button")](http://www.mailbeez.com/wp-content/uploads/2011/03/edit_button.png)"Edit Content" Button

 

Das Plugin funktioniert mit allen kostenlosen und kostenpflichtigen Modulen und sogar mit selbst entwickelten, so lange diese das MailBeez Template System verwenden.

Der Editor unterstützt den Bearbeitungsvorgang mit Vorschau-Buttons für die html & txt version. Auch können Test-Emails direkt aus der Bearbeitungsansicht versendet werden.

Funktionen

- Automatischer Import der Vorlagen (.tpl Dateien)
- komfortables Bearbeiten mit Vorschau und Test-Versand
- Wiederherstellungsfunktion des Standard-Templates für den Notfall
- Vorlagen werden in der Datenbank gespeichert, somit einfaches Update der Module

Der Vorlagen Manager ist voll kompatibel zum [Multilanguage Template Manager](/documentation/configbeez/config_tmplmngr_lng/ "Multilanguage Template Manager"), falls der Shop mehrsprachig werden soll.

Entwicklungs Roadmap:

- Syntax Highlighting for html and template variables
- buttons to insert available template variables
- layout view for editing

 
