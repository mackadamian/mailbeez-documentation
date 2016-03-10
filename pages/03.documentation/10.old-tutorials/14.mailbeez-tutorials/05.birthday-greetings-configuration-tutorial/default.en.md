---
# http://learn.getgrav.org/content/headers
title: Birthday Greetings
slug: birthday-greetings-configuration-tutorial
# menu: Birthday Greetings
date: 11-07-2012
published: true
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

This awesome and completely free email marketing module will send birthday greetings to your customers. This reminds customers that they’ve shopped with you before and communicates your appreciation via remembrance of their special day – all whilst having a zero impact on your marketing budget!

If you want to kick it up a notch, you can include a gift from your store in the form of a personalized coupon embedded into the Birthday Greeting email with the [MailBeez Birthday Coupon module.](/documentation/mailbeez/coupon_birthday/) Sweet!

## Getting Started


1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png&w=270&h=112&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Locate the Birthday Greetings module and click on it.
2. If you followed the MailBeez Installation instructions, you should see this:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/birthday/birthday_config1.png&w=155&h=396&zc=1&q=100 "Birthday Greetings Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/birthday/birthday_config1.png "Birthday Greetings Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

If not, you will see this and will need to click on the “Install” button:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/birthday/birthday_config2.png&w=175&h=122&zc=1&q=100 "Install Birthday Greetings")](http://www.mailbeez.com/images/doc/mailbeez/birthday/birthday_config2.png "Install Birthday Greetings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

## Configuring the Birthday Greetings Module

There are 5 function buttons and 8 configurable settings. We will go through each of them one at a time.

### General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/birthday/birthday_config3.png&w=175&h=359&zc=1&q=100 "Birthday Greetings General Settings")](http://www.mailbeez.com/images/doc/mailbeez/birthday/birthday_config3.png "Birthday Greetings General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Target Days Before & Target Days After**  
In earlier versions of this module, these settings are “set days before” and “set days to skip after”. The concept is the same, but the language has been updated for ease of use.

These settings work together to create a window of time in which MailBeez will look for opportunities to send the Birthday Greeting email by targeting customers who fall within the time frame you create with these settings.

**Target Days Before**  
 This setting lets you target customers “X” number of days before their birthday. It is set to “1” by default, meaning that when this module is run, MailBeez will target customers who have a birthday 1 day in the future.

If you want customers to receive the Birthday Greeting emails earlier than 1 day ahead of their birthday, change this setting to a higher number.

**Target Days After**  
 This setting lets you target customers who had a birthday “X” number of days in the past. By default it is set to “2”, meaning that when this module is run, MailBeez will target all customers who had a birthday within the past 2 days.

The default settings of 1 day before and 2 days after creates a 4 day window of time (1 day before + today + 2 days after = 4 days). When the module is run with these settings, MailBeez will find and send an email to all customers who have a birthday falling within that window and who have not yet received the Birthday Greeting email.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

### Google Analytics Settings

The ability to configure Google Analytics tracking on a per-module basis has been deprecated. The Google Analytics settings selected in the Basic Configuration section apply to all modules. This setting will be removed in the next release.

**Google Analytics Integration**  
 When you configured your MailBeez software, one of the steps guided you through configuring your Google Analytics Integration settings. If you turned on Google Analytics Integration in your Basic Configuration settings, this setting will allow you to control whether it is turned off or on for this particular module.

It is set to “True” by default, meaning it is turned on for this module. If you desire, you can turn it off for this module without affecting the other modules Google Analytics are used with.

**Google Analytics Integration URL rewrite mode**  
 This setting allows you to control your Google Analytics URL Rewrite Mode. It is set to “default”, meaning it pulls the Google Analytics Integration URL rewrite mode setting you selected in the Basic Configuration section.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!

## Test & Run the Birthday Greetings Module

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
