---
# http://learn.getgrav.org/content/headers
title: Nopurchase Simple
slug: ID-4426
# menu: Nopurchase Simple
date: 11-07-2012
published: false
publish_date: 11-07-2012
# unpublish_date: 11-07-2012
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

This MailBeez Module allows you to contact customers who have created an account but have never made a purchase. You can edit the language in the email templates to encourage customers to shop with you, request feedback about their hesitation to purchase, or tell them about sales and specials to tempt them to make a purchase!

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

If you want to kick it up a notch, you can include a coupon in your emails to entice customers back to your store by installing the [MailBeez Nopurchase Advanced module!](/documentation/mailbeez/nopurchase_advanced/)

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png&w=270&h=112&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Nopurchase Simple module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_simple/nopurchase_simple_config1.png&w=175&h=151&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_simple/nopurchase_simple_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration settings are now available for you to edit

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_simple/nopurchase_simple_config2.png&w=149&h=396&zc=1&q=100 "Nopurchase Simple Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_simple/nopurchase_simple_config2.png "Nopurchase Simple Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring the Nopurchase Simple Module

There are 5 function buttons and 7 configurable settings. We will go through each of them one at a time.

### General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_simple/nopurchase_simple_config3.png&w=175&h=320&zc=1&q=100 "Nopurchase Simple General Settings")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_simple/nopurchase_simple_config3.png "Nopurchase Simple General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Target Days Without Purchase & Target Days to Look Back**  
In earlier versions of this module, these settings are “Nopurchase delay” and “Set number of days to skip processing”. The concept is the same, but the language has been updated for ease of use.

These settings work together to create a window of time in which MailBeez will look for opportunities to send the Nopurchase email by targeting customers who fall within the time frame you create with these settings.

**Target Days Without Purchase**  
 This setting lets you target customers who have created an account but have not made a purchase after “X” number of days. By default it it set to 5, meaning that if a customer creates an account and still has not made a purchase 5 days later, MailBeez will target them for a Nopurchase email when the Nopurchase module is run.

If you want to give your customers more time to make a purchase before sending out the Nopurchase email, simply increase this number. Conversely, if you want to give them less time without a purchase before contacting them, you will lower this number.

**Target Days to Look Back**  
 This setting lets you define how far back in time MailBeez should look for customers who meet the Days Without Purchase criteria. By default, it is set to 10 and must always be a higher number than the “Target Days Without Purchase” setting.

The default settings of 5 Days Without Purchase and 10 Days to Look Back work together to tell MailBeez “Search my database for the last 10 days and find all customer accounts that were created but show no purchases made after 5 days, and send them a Nopurchase email.”

Since Days to Look Back is set to 10, and Days Without Purchase is set to 5, this means MailBeez will find 2 batches of customers who meet the Days without Purchase criteria (10 divided by 5 = 2).

This is important because if a run of this module fails and a batch of customers are missed, they will get picked up in the next run. So it is a good idea to set Target Days to Look Back to be double Target Days Without Purchase. For example, if you change Target Days Without Purchase to 3, then you would want to change Target Days to Look Back to 6.

MailBeez will disregard customers who meet the criteria of these two settings who have already received a Nopurchase email, ensuring that a customer will not receive the same email twice.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Check For Empty Customer Basket**  
 This setting lets you choose whether or not to target only those customers with an empty basket or shopping cart. It is set to “False” by default, meaning it will target all customers who have created an account but not made a purchase whether they have products in their basket or not. Changing this setting to “True” will result in targeting only the nopurchase customers who have an empty basket.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!  
  

### Test & Run the Nopurchase Simple Module

The 5 function buttons are the controls that allow you to test the module and then manually run it when you’re ready:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/function_buttons.png&w=175&h=184&zc=1&q=100 "Function Buttons")](http://mailbeez.com/images/doc/common_images/function_buttons.png "Function Buttons")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Email Templates – “HTML” Button**  
 This button allows you to preview the module templates in a nice popup window in HTML format. This way, you can easily see what the email template looks like and quickly determine which aspects of the template you’ll want to customize for your use.

As you modify your template files, you can come back and use this button to view your changes to ensure that they are appearing as you intend.

**When you’re ready to customize your email templates, have a look at our [Customizing Free Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-free-email-templates/)**

**Email Templates – “TXT” Button**  
 This button allows you to preview the module templates in a nice popup window in text format. Everyone has customers who prefer to receive email in text format. This tool allows you to see what they see, and preview changes you make to the template before they go out to your customers.

**Recipients – “Show” Button**  
 Clicking this button will result in a nice popup window in your admin which is populated with a list of everyone who is getting this email in the next run. (Depending on the “early check” setting you will see all or new recipients only)

**Send Test Email – “Send” Button**  
 This button does just what it says – it lets you send a test email with test data.

**Run this module – “Run” Button**  
 This is the button you use to actually run the module. This button respects your run mode as it is set in your Simulation Configuration, so if you’re in Simulation Mode, clicking this button results in a simulation run. If you are in Production Mode, clicking this button results in a production run.

It even tells you in the text above the button which mode you’re in. This prevents you from accidentally sending emails out to customers when you’re testing.



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.

## Template Manager

Mailbeez has developed a handy module that easily allows you to both edit and view your text changes right from the MailBeez interface within your store’s admin. Fully functional with all official MailBeez Modules (free, premium, and custom built), the MailBeez Template Manager makes editing a template a breeze, so much so that you may wonder how you ever lived without it! **[ Learn more!](/documentation/configbeez/config_tmplmngr/)**
