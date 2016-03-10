---
# http://learn.getgrav.org/content/headers
title: Winback Simple
slug: ID-4441
# menu: Winback Simple
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

This MailBeez Module allows you to contact customers who have not made a purchase in a while. You can edit the language in the email templates to encourage customers to revisit you and see what’s new, or to tell them about sales and specials that may tempt them to come back and make a purchase!

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

If you want to kick it up a notch, you can include a coupon in your emails to entice customers back to your store by installing the [MailBeez Winback Advanced module!](/documentation/mailbeez/winback_advanced/)

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png&w=270&h=112&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Winback Simple module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_simple/winback_simple_config1.png&w=175&h=206&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/winback_simple/winback_simple_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration settings are now available for you to edit

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_simple/winback_simple_config2.png&w=139&h=396&zc=1&q=100 "Winback Simple Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/winback_simple/winback_simple_config2.png "Winback Simple Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring the Winback Simple Module

There are 5 function buttons and 7 configurable settings. We will go through each of them one at a time.

### General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_simple/winback_simple_config3.png&w=175&h=320&zc=1&q=100 "Winback Simple General Settings")](http://www.mailbeez.com/images/doc/mailbeez/winback_simple/winback_simple_config3.png "Winback Simple General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Target Order Status, Target Days Since Last Purchase, & Target Days to Look Back**  
In earlier versions of this module, these settings were “Set order status’, ‘Winback Delay”, and “Set number of days to skip processing’. The concepts are the same, but the language has been updated for ease of use.

These 3 settings work together to identify eligible customers & create a window of time in which MailBeez will look for them when the Winback module is run.

**Target Order Status**  
 This setting lets you define the order status an order must have for the customer to be targeted to receive a Winback email. By default, it is set to an order status of “Delivered”, “Shipped”, or “Dispatched”, depending on your e-commerce platform. Customers who have an order status that matches this setting and who fall within the time frame parameters defined in the next two settings will receive a Winback email when this module is run.

**Target Days Since Last Purchase**  
 This setting tells MailBeez to target orders “X” number of days after their last order reaches the required order status as defined by the “Target Order Status” setting. By default it is set to “180”, meaning that orders which have reached “Target Order Status” 180 or more days ago will be eligible to receive a Winback email when the Winback module is run.

**Target Days to Look Back**  
 This setting lets you define how far back in time MailBeez should look for customers who meet the Order Status and Days Since Last Purchase criteria. By default, it is set to 200 and must always be a higher number than the “Target Days Since Last Purchase” setting.

**How it Works & Changing Settings**  
 The default settings of: Order Status = Delivered, Days Since Last Purchase = 180, and Days to Look Back = 200 all work together to tell MailBeez “Search my database for the past 200 days and find all orders which have reached a status of Delivered 180 or more days ago, and send them a Winback email.”

MailBeez will disregard customers who meet the criteria of these 3 settings who have already received a Winback email, ensuring that a customer will not receive the same email twice.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!  
  

### Test & Run the Winback Simple Module

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
