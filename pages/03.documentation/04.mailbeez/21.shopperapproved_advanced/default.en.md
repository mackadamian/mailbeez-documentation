---
title: 'Shopper Approved Advanced'
slug: shopperapproved_advanced
date: 08-05-2015
published: true
publish_date: 08-05-2015
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
    tag:
        - pro
module:
    code: shopperapproved_advanced
    category:
        - mailbeez
    compatiblity:
        - comp_osc
        - comp_cre
        - comp_digi
        - comp_zencart
        - comp_xtc
        - comp_gambio
    thumbnail: 'http://www.mailbeez.com/wp-content/uploads/downloads/thumbnails/2013/06/top_64.png'
    pro: pro
    cert: 'true'
    price: '99 EUR'
    title_en: 'Shopper Approved Advanced'
    teaser_en: 'Advanced Features: Delay for international orders, multiple Order status, recognition of regular customers'
    title_de: 'Idealo Profi'
    teaser_de: 'Profi-Features: Verzögerung für internationale Bestellungen, Stammkunden-Erkennung und mehr'
    author: MailBeez.com
author:
    name: admin
metadata:
    author: admin
---

**Get most out of your Shopper Approved Plan**

This module allows to invite your Customers to review your Store on Shoppperapproved.com - also you can go back in time to kickstart your reviews!

## Advanced Features

This advanced module gives you a couple of settings to streamline and improve your process of inviting customers to give a rating on Shopper Approved:

## multiple order status

Do you have different order status marking orders as shipped! No problem, just check all orders status you want the module to react on

## delay times for international orders

Shipping to international customers typically takes a couple days longer. To avoid sending a rating invite before delivery, you can define an additional delay for orders shipping to other countries than your own!

The module automatically applies this delay to all orders which are shipped to a country, which is different from the country you configured in your store system.

## recognition of regular customers

Don't want to bother your regular customers with an Email to rate on Shopper Approved? Simply define a delay (e.g. 120 days) between to invites and your are done. The module will check when the last invite was sent and decides whether to wait or to send a new rating invite.

## Segmentation by number of orders

Select how many Orders a customer must have place before the module invites for giving a rating!

### Want to integrated your valuable ratings with your Store and Email Marketing?

Using the [Shopper Approved Integration Suite](/documentation/configbeez/config_shopperapproved_integration/) you can easily integrate your Reviews with your Store - in a way that makes this "unique fresh content" visible to search engines - and your MailBeez generated Email Marketing emails!

## Different Ways to invite - adoptable to your needs!

### Invite to initial Survey with pre-populated customer data

## default review page

The default review page is template based and you can easily set up your own, customized template!

### make any page a review page

insert the following code on the page (e.g. `my-custom-page.php`) you want to direct the customers to place a review

```
if (isset($_GET['SA'])) {
    require_once(DIR_FS_CATALOG . 'mailhive/mailbeez/shopperapproved_advanced.php');
    $sa = new shopperapproved_advanced();
    $code = $sa->generate_page($_GET['SA'], 'core.tpl.html');
    echo $code;
}
```


and adjust the invite link in your MailBeez Email template to e.g.

`http://mydomain.com/my-custom-page.php?SA={$sa_invite_parameter_value}`

## Invite to full Survey with pre-populated order-id

Do you want to skip the initial survey? No Problem!

Copy the link to full surveys from your shopper approved account into your MailBeez email template and replace `<order-id>` with `{$order_id}`

Now customers are directed to the full surver with pre-filled order id!
