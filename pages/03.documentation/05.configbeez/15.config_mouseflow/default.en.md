---
title: 'Mouseflow Integration'
slug: config_mouseflow
date: 20-10-2011
published: true
publish_date: 20-10-2011
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
        - core
author:
    name: admin
metadata:
    author: admin
---

## What is Mouseflow?

[Mouseflow](http://shrsl.com/?~6plv) is a web service that gathers data & presents it as heat maps, telling you which areas of your site are getting the most attention by your visitors. Areas being overlooked by users can then be improved to gain more attention.

  
 The MailBeez Mouseflow Integration module works with your existing Mouseflow installation to allow you to track visitors arriving to your site from links within all of your MailBeez generated emails.

Visit [Mouseflow](http://shrsl.com/?~6plv) to register and get **100 monthly recordings free**.

## Mouseflow Features

[Mouseflow](http://shrsl.com/?~6plv) can actually record a visitor’s activity on your site in real time. This can greatly help you in determining the user friendliness of your site and how visitors interact with the available tools.

- Watch how your visitors are using your website – seconds after they visited.
- See all mouse movements, clicks, scroll events, key strokes and form interactions.
- Discover problematic parts of your website and learn how to enhance the user experience.
- Get a visual overview of the clicks received by your pages.
- Compare heatmaps from different periods to measure the effects of changes made to the website.
- Simple installation – insert a single line of Javascript into your storefront
- And [many more…](http://shrsl.com/?~6plv)

**See all [Mouseflow features](http://shrsl.com/?~6plv)**

Mouseflow offers a variety of monthly plans designed to fit every budget and need. The free plan allows monitoring of 1 website with up to 100 monthly recordings which are stored for 1 month.

Need more? How about monitoring of 3 websites with up to 10.000 monthly recordings which are stored for 2 months for only 49Eur/month? The reasonable pricing and superb performance is what makes this Mouseflow’s most popular plan!

## MailBeez and Mouseflow – A Powerful Combination

Insert the following PHP code into your `includes/application_bottom.php` and configure your custom tracking code to get the Mouseflow Integration module to do everything for you that Mouseflow does!

```
// MailBeez
if (defined('MAILBEEZ_MOUSEFLOW_STATUS') && MAILBEEZ_MOUSEFLOW_STATUS == 'True') {
    require_once(DIR_FS_CATALOG . 'mailhive/configbeez/config_mouseflow/includes/mouseflow_inc.php');
}
// - MailBeez
    
```


Additionally, integrating MailBeez with Mouseflow lets you control what kind of users you would like to record so you can keep your costs down:

- Activate/De-activate the module as desired
- Include or exclude visitors coming through MailBeez Email campaigns
- Limit recordings to only those visitors coming through MailBeez Email campaigns
- Exclude Administrators by IP so you don’t pay for recordings from visits by you or your employees

Keeping costs low doesn’t mean having to sacrifice getting the data you need! With the MailBeez Mouseflow Integration module, get answers to such questions as:

- Which steps do customers perform when asked to write a review? Is your review process easy & friendly?
- How to customers react to Winback campaigns? Do you need to change the verbiage in my Winback emails?
- How do coupons influence your customers behavior? Do your coupons need tweaking?
- Are you seeing a sales result from the Birthday Greeting module, or do you need to upgrade to the Birthday Coupon module?

With the MailBeez Mouseflow Integration module, you can improve your MailBeez Email campaigns, optimize your landing pages to your visitor’s behavior, and identify new & better ways to make MailBeez work for you!


