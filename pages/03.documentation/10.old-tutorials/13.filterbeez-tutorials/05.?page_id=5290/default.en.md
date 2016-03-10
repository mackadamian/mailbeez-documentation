---
# http://learn.getgrav.org/content/headers
title: Extended Customer Information
slug: ID-5290
# menu: Extended Customer Information
date: 08-08-2012
published: false
publish_date: 08-08-2012
# unpublish_date: 08-08-2012
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
# added collection selector

author:
    name: kelly
metadata:
    author: kelly
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

The screenshots used in this tutorial were made using Zen Cart. If you use a different e-commerce platform, your admin interface and MailBeez interface may appear slightly different, however the concepts and configuration instructions are the same across all platforms.

 

## About This Module

This module lets you add a variety of additional customer information into your emails so that each customer will receive personalized emails that provide the impression that the mailings you send them are customized just for them, vs. an impersonal bulk mailing that goes out to a massive mailing list. For example, in addition to displaying the customer’s name in your emails, you can also display their date of birth, phone number, company name, address, fax number, newsletter subscription status, and more!

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Filter & Helper tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/filter_tab.png&w=270&h=85&zc=1&q=100 "Filter & Helper Tab")](http://www.mailbeez.com/images/doc/common_images/filter_tab.png "Filter & Helper Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Add Extended Customer Information module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_add_customer_information/extend_customer_info_config1.png&w=175&h=206&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/filterbeez/filter_add_customer_information/extend_customer_info_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration settings are now available for you to edit:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_add_customer_information/extend_customer_info_config2.png&w=175&h=367&zc=1&q=100 "Add Extended Customer Information Configuration Panel")](http://www.mailbeez.com/images/doc/filterbeez/filter_add_customer_information/extend_customer_info_config2.png "Add Extended Customer Information Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring the Module

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on second “Edit” button at the bottom of the configuration panel
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to work once you edit your email template files.

### Configure General Settings

Since the Add Extended Customer Information module is already activated by default, no further configuration of the module is necessary. If you need to deactivate the module for any reason, navigate to MailBeez > Filter & Helper tab > Add Extended Customer Information, the topmost “Edit” button, and change the setting to “False”.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_add_customer_information/extend_customer_info_config3.png&w=175&h=101&zc=1&q=100 "Add Extended Customer Information General Settings")](http://www.mailbeez.com/images/doc/filterbeez/filter_add_customer_information/extend_customer_info_config3.png "Add Extended Customer Information General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## How Do I Use the Module?

It’s so easy! All you have to do is add any of the template variables listed below to any email template in which you wish to display the corresponding customer information.

 Template Variable Customer Information  {$data.customer.firstname} First Name  {$data.customer.lastname} Last Name  {$data.customer.dob} Date of Birth  {$data.customer.telephone} Phone Number  {$data.customer.fax} Fax Number  {$data.customer.newsletter} Newsletter Subscription Status (0/1)  {$data.customer.company} Company  {$data.customer.postcode} Post Code  {$data.customer.city} City  {$data.customer.state} State  {$data.customer.country\_id} Country ID  {$data.customer.zone\_id} Zone ID  {$data.customer.raw} An array of all the above information  

## How Do I Edit My Email Templates?

You do need to be able to customize your MailBeez templates to utilize this add on, so if you do not feel confident making these edits yourself, or feel you do not have enough experience with this, you can [get some professional MailBeez support](http://www.mailbeez.com/support/service/) or have a look at our tutorial on [Customizing MailBeez Premium Email Templates](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.
