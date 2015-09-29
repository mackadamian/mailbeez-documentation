---
# http://learn.getgrav.org/content/headers
title: Gutschein Generator
slug: config_coupon_engine
routes:
    default: /dokumentation/configbeez/config_coupon_engine
    aliases:
        - /dokumentation/configbeez/gutschein-generator
        
# menu: Gutschein Generator
date: 10-04-2012
published: true
publish_date: 10-04-2012
# unpublish_date: 10-04-2012
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
    tag: [pro]
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

eine Übersicht der unterstützen Shopsystem findet sich auf [MailBeez Kompatibilität](/dokumentation/compatibility/).

## osCommerce Gutschein System Unterstützung

Als “Mutter” aller eCommerce Systeme ist osCommerce als sauberes Kern-System angelegt und besitzt kein Gutschein System.  
 Wahrscheinlich haben Sie bereits ein Gutschein System in osCommerce installiert. MailBeez unterstützt eine Reihe von Gutschein-Systemen wie nachfolgende aufgelistet. Die Tabellen-Namen helfen, das installierte System zu identifizieren.

### CCGV basierte Gutschein Systeme

Es gibt eine Reihe von Gutschein Systemen, welche vom “CCGV” Addon abstammen:

wie http://addons.oscommerce.com/info/4135  
 oder http://addons.oscommerce.com/info/282  
 oder http://addons.oscommerce.com/info/8002  
 oder http://addons.oscommerce.com/info/9020 (osc 2.3.3.4)

Tables:  
 TABLE\_COUPONS, TABLE\_COUPONS\_DESCRIPTION, TABLE\_COUPON\_EMAIL\_TRACK, TABLE\_COUPON\_REDEEM\_TRACK (, TABLE\_COUPON\_RESTRICT)

### Discount Coupon Codes

http://addons.oscommerce.com/info/4269

Tables:  
 TABLE\_DISCOUNT\_COUPONS, TABLE\_DISCOUNT\_COUPONS\_TO\_ORDERS, TABLE\_DISCOUNT\_COUPONS\_TO\_CATEGORIES, TABLE\_DISCOUNT\_COUPONS\_TO\_PRODUCTS, TABLE\_DISCOUNT\_COUPONS\_TO\_MANUFACTURERS, TABLE\_DISCOUNT\_COUPONS\_TO\_CUSTOMERS, TABLE\_DISCOUNT\_COUPONS\_TO\_ZONES

### Discount Coupons by high-quality-php-coding.com

http://high-quality-php-coding.com

Tables:  
 TABLE\_DISCOUNT\_CODES, TABLE\_CUSTOMERS\_TO\_DISCOUNT\_CODES
