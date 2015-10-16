---
title: 'Coupon Engine'
slug: config_coupon_engine
routes:
    default: /documentation/configbeez/config_coupon_engine
    aliases:
        - /documentation/configbeez/coupon-engine
date: 10-04-2012
published: true
publish_date: 10-04-2012
template: docs
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: done
    category:
        - docs
    tag: [pro,coupon]
module:
    code: 'pro'
    category: [pro]
    compatiblity: [comp_cre,comp_digi,comp_zencart,comp_xtc,comp_gambio]   
    pro: 'pro'     
author:
    name: admin
metadata:
    author: admin
---

Find an overview of the store compatibility on: [MailBeez Compatibility](/documentation/compatibility/).

The MailBeez Coupon Engine is a sub-module utilized by any MailBeez module which sends out personalized coupons.



###Advantages of personalized coupons

In comparison to static coupon codes (e.g. "BIRTHDAY") there are a number of advantages using personlized coupons:

- **no unwanted viral effect**: You can configure how often a coupon can be applied
- **Sense of urgency due to expiry date**: Each generated coupon has an expiry date, e.g. 14days starting with the day the coupons was sent. The expiry date creates a sense of urgency leading to more orders. In addition you can utilize the [Coupon Expiry Reminder](/documentation/mailbeez/coupon_expire) to follow-up a couple of days before the expiry date - great for conversion!
- **Traceability**: The system can connect the coupon code to the receiving customer and the email it was sent with. That allows you to understand the effect of your coupons and emails.



###Template Coupons

The coupon engine generates personalized coupons based on **template coupons** which are assigned to the according email modules.
 
A **template coupon** is a "normal" coupon, but distinguishes through the coupon **CODE**, which **MUST** start with the pattern `template_`.

>>>>>>Make sure to run the tour how to set up a template coupon
 
**Example "[Birthday Coupon](/documentation/mailbeez/coupon_birthday)"**:

As the first step create a new coupon with 

CODE = `template_birthday`

and enter the values accordingly (e.g. 10% off) - the expiry date is not used.

In module [Birthday coupon](/documentation/mailbeez/coupon_birthday) you can now assign this template coupon (remember to save your settings).

During the generation process of birthday emails a personalized coupon is generated for every recipient base on the settings of the template coupon. In addition there will be generated a random coupon code and a dynamic expiry date - e.g. 14days after date of sending.

You can test the setup by running a simulation: In Simulation-Mode please execute the module. This will generate "real" emails with "real" coupons, which are not sent to your customers but to your configured simulation email address. This allows you to validate the coupon settings and even try to place a test-order.



###Maintainance features

In this module you find a range of features which will help you to maintain your coupons:
 

**Coupon Search**: Find a coupon and edit it, also available as [Dashboard-Widget](/documentation/dashboardbeez/dashboard_coupon_admin) zur Verfügung.

**Delete Simulation Coupons**: When running a simulation "real" coupons are generated. This button allows you to clean up the mess ;)

**Delete expired Coupons**: Clean up expired coupons

**Repair sync**: In case coupons are not assigned to message you can repair this assignment


>>>>>**Please note**: In each module you can configure the length of the coupon code. Long codes (e.g. 8 or 10 characters) can be generated very efficiently. With short code-length and many existing codes the system my need to "try" for a longer time until a free code is found. This can cause issues like time outs of the sending process.

## osCommerce Coupon System support

As the “mother of all eCommerce System", osCommerce is kept as a clean core without having addons like a coupon system.  
 You probably have already added a coupon system to osCommerce and MailBeez supports a number of different coupon systems as listed below. The table names listed might help you to identify, which coupon system you are using.

In case you have not yet install a coupon engine we recommend a CCGV based addon.

### CCGV based coupon systems

There are a number of coupon system addons based on the “CCGV” coupon system, e.g.:

- [http://addons.oscommerce.com/info/4135](http://addons.oscommerce.com/info/4135)  
- [http://addons.oscommerce.com/info/282](http://addons.oscommerce.com/info/282)  
- [http://addons.oscommerce.com/info/8002](http://addons.oscommerce.com/info/8002)  
- [http://addons.oscommerce.com/info/9020](http://addons.oscommerce.com/info/9020) (osc 2.3.3.4)

These addons utilize an almost identical database structure

**Tables**:

You should find following tables in your table definition in case you are using a CCGV based coupon engine

```bash
TABLE_COUPONS
TABLE_COUPONS_DESCRIPTION
TABLE_COUPON_EMAIL_TRACK
TABLE_COUPON_REDEEM_TRACK
TABLE_COUPON_RESTRICT
 
```

#### Discount Coupon Codes

[http://addons.oscommerce.com/info/4269](http://addons.oscommerce.com/info/4269)

**Tables**:

You should find following tables in your table definition in case you are using a DCC based coupon engine


```bash
TABLE_DISCOUNT_COUPONS
TABLE_DISCOUNT_COUPONS_TO_ORDERS
TABLE_DISCOUNT_COUPONS_TO_CATEGORIES
TABLE_DISCOUNT_COUPONS_TO_PRODUCTS
TABLE_DISCOUNT_COUPONS_TO_MANUFACTURERS
TABLE_DISCOUNT_COUPONS_TO_CUSTOMERS
TABLE_DISCOUNT_COUPONS_TO_ZONES
 
```

#### Discount Coupons by high-quality-php-coding.com

[http://high-quality-php-coding.com](http://high-quality-php-coding.com)

**Tables**:

Wenn Sie ein DC basiertes Gutschein System nutzen, sollten Sie folgende Tabellen in der Tabellen-Definition finden:



```bash
TABLE_DISCOUNT_CODES
TABLE_CUSTOMERS_TO_DISCOUNT_CODES

```

