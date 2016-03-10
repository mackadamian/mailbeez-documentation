---
# http://learn.getgrav.org/content/headers
title: MailBeez Check for Updates
slug: mailbeez-check-for-updates-configuration-tutorial
# menu: MailBeez Check for Updates
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

This MailBeez Module checks your system against the MailBeez-Server for updates or new Modules and sends you an Email with the result.

The email is formatted as a nice little report that tells you how many MailBeez emails you’ve sent out so far, and which – if any – of your modules need updating. It will also advise you when updates to your core MailBeez software are available.

For your convenience, it will also display a list of MailBeez modules which are available but not yet installed. If you have a webmaster or site administrator who manages your store for you, you can forward this email to them as a status report or to do list. Handy!

Alternatively, you may [use the MailBeez Version Check widget ](/documentation/tutorials/using-the-mailbeez-version-check-widget/) to check for updates.

## Getting Started


1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png&w=270&h=112&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Locate the MailBeez Version Check module and click on it.
2. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/mailbeez_check/updateMB_config1.png&w=175&h=89&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/mailbeez_check/updateMB_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration settings are now available for you to edit

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/mailbeez_check/updateMB_config2.png&w=175&h=326&zc=1&q=100 "Version Check Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/mailbeez_check/updateMB_config2.png "Version Check Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

## Configuring the Version Check Module

There are 5 function buttons and 4 configurable settings. We will go through each of them one at a time.

### General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/mailbeez_check/updateMB_config3.png&w=175&h=323&zc=1&q=100 "Version Check General Settings")](http://www.mailbeez.com/images/doc/mailbeez/mailbeez_check/updateMB_config3.png "Version Check General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “True” by default, meaning the module is on and ready to work. Change this setting to “False” to deactivate the module and disable it from being run.

**Sender and Receiver Email**  
 This setting lets you control the email address that is used to send and receive the update results email. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

Because this is a shared setting, meaning it is used as both the send to and receive from email address, your update results emails will be from “YourStoreEmail@yoursite.com” to “YourStoreEmail@yoursite.com”.

**Sender and Receiver Name**  
 This setting lets you control the sender and receiver name that is displayed as the sender and receiver in your update results email. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

Because this is a shared setting, meaning it is used as both the sender and receiver name, your update results emails will be from “Your Store Name” to “Your Store Name”.

**Interval**  
 This setting allows you to choose the interval at which the module will check for updates. Your choices are every day, every week, or every month. By default, it is set to check for a week at a time. You should adjust this setting based on how often you plan to run the module.

To run this module automatically based on the interval setting you select, you will need to either set up a cronjob on your server or Install the simple and affordable [Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!

### Test & Run the Check For Updates Module

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

Now that you know how to use the Check For Updates email module to identify which modules need updating, let’s talk briefly about how to actually update the modules.

## How to Update MailBeez Modules

Each module comes with a step-by-step update.txt file that walks you through the process. You will see that updating MailBeez modules is quick and easy. Once you’ve run the Check for Updates email module to identify which of your modules need updating, follow these simple steps:

### Updating Free MailBeez Modules


- In the email, click on the “Read More” link next to the module that needs updating to go to the module’s page on the MailBeez website

Alternatively, if you set the “Show Email While Sending” to “True” when you completed your basic configuration, then the popup will display the same information as the email this module generates, and you can click the “Read More” link from there. This comes in very handy in situations where the email is configured to go to someone other than you, such as an administrator or webmaster.

- Download the fileset & unzip it on your computer
- Using FTP, navigate to that mod’s template files and download your customized versions
- Replace the template files in the fileset with the customized versions you just downloaded
- Follow the step-by-step instructions in the upgrade.txt file included in the fileset so you’ll know which module files need replacing

### Updating Premium MailBeez Modules

- Download the updated fileset from Avangate using the download link from the delivery email. If you have lost this information, log in to your account at avangate.com and download from there.
- Unzip the downloaded fileset on your computer
- Using FTP, navigate to that mod’s template files and download your customized versions
- Replace the template files in the fileset with the customized versions you just downloaded
- Follow the step-by-step instructions in the upgrade.txt file included in the fileset so you’ll know which module files need replacing



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.

## Template Manager

Mailbeez has developed a handy module that easily allows you to both edit and view your text changes right from the MailBeez interface within your store’s admin. Fully functional with all official MailBeez Modules (free, premium, and custom built), the MailBeez Template Manager makes editing a template a breeze, so much so that you may wonder how you ever lived without it! **[ Learn more!](/documentation/configbeez/config_tmplmngr/)**
