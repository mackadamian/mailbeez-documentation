---
# http://learn.getgrav.org/content/headers
title: Numinix Store Credit: Balance Reminder
slug: ID-6197
# menu: Numinix Store Credit: Balance Reminder
date: 20-09-2012
published: false
publish_date: 20-09-2012
# unpublish_date: 20-09-2012
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

Requirements:

- The Numinix Store Credit & Reward Points addon for Zen Cart
- Zen Cart e-commerce platform

The Numinix Store Credit Balance Reminder module will periodically send a store credit balance reminder to your customers.

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Numinix Store Credit Balance Reminder module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/install.png&w=175&h=78&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/numinix_balance_reminder_config.png&w=175&h=680&zc=1&q=100 "Numinix Store Credit Balance Reminder Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/numinix_balance_reminder_config.png "Numinix Store Credit Balance Reminder Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configure the Balance Reminder Module

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/general_settings.png&w=175&h=475&zc=1&q=100 "Numinix Store Credit Balance Reminder General Settings")](http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/general_settings.png "Numinix Store Credit Balance Reminder General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Minimum Balance Amount, Minimum & Maximum Days to Delay Sending**  
 These settings work together to create a window of time in which MailBeez will look for opportunities to send the Balance Reminder email by targeting customers who meet the criteria you define with these settings.

**Minimum Balance Amount**  
 This setting lets you define the lowest store credit balance a customer must have in order to be eligible to receive a Balance Reminder email. By default, it is set to “10″, meaning that only customers with a store credit balance of $10 or more will receive a Balance Reminder email when this module is run.

**Minimum Days to Delay Sending**  
 What is the least amount of time MailBeez should wait after the Review Reward email is sent before sending a Balance Reminder email? By default, this is set to “30″, meaning that this module will target customers who have received a Review Reward email no less than 30 days ago.

Leaving it set to “30″ will result in the Balance Reminder email being sent every 30 days as a monthly reminder.

**Maximum Days to Delay Sending**  
 What is the most amount of time MailBeez should wait after the Review Reward email is sent before sending a Balance Reminder email? By default, it is set to “40″, meaning that this module will target customers who have received a Review Reward email no more than 40 days ago.

The default settings tell MailBeez, “Search my database for all customers who have a store credit balance of $10 or more. Of those, find which ones have received a Review Reward email between 30 and 40 days ago and send them a Balance Reminder email”.

**Limit Number of Emails per Run**  
 The first time you run this module, all of your customers meeting the Minimum Balance Amount criteria will receive a Balance Reminder email. Since most web hosts place limits on how many emails you can send out per hour, you will need to check with your hosting company to find out if this is true for you. If it is, you will need to place a limit on how many emails this module sends per hour.

There are two ways to do this. You can either add the [Simple Throttling module](/documentation/filterbeez/filter_do_throttling_simple/) to your MailBeez installation, or you can use this setting to define how many emails this module should send per hour, based on your web host limitations. Then, you will need to run this module every hour until all of the emails have been sent.

By default, this setting is 100, but again you should check with your web host and configure this setting accordingly.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Layout**  
 This setting allows you to choose which layout style template set you want to assign & use for this module.

Since the Numinix Store Credit Balance Reminder module does not include additional templates, the only option displayed here is “Default” until such a time as you create your own custom templates. For help creating your own custom templates, check out our [Customizing Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

 

## Install & Configure the Numinix Store Credit Display Balance Filter

The Numinix Store Credit Balance Reminder module adds a new filter to your MailBeez installation: the Numinix Store Credit Display Balance filter.

This filter allows you to display the customer’s current store credit balance in any MailBeez generated email.

1. Navigate to the Filter & Helper tab of your MailBeez User Interface
2. Click on the Numinix Store Credit Display Balance filter and then click its ‘Install’ button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/filter_install.png&w=175&h=141&zc=1&q=100 "Install the Filter's Configuration Settings into Your Database")](http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/filter_install.png "Install the Filter's Configuration Settings into Your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Click on the “Edit” button to bring up the filter’s configuration panel:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/filter_config.png&w=175&h=242&zc=1&q=100 "Numinix Store Credit Display Balance Filter Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/numinix_sc_balance_reminder/filter_config.png "Numinix Store Credit Display Balance Filter Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

You may leave these settings as they are unless you want to change them:

**How It Works**  
 To use this filter, simply add this bit of code into any MailBeez email template in which you want the customer’s store credit balance to appear:

{$content.numinix\_sc\_balance}

   
 If you want it to appear in all emails generated by MailBeez, place it in the footer of the main template. If you prefer to select which emails display this data, place the code within the individual module templates.

**The customer’s store credit balance is already displayed in the emails generated by the Numinix Store Credit Balance Reminder & the Numinix Store Credit Review Rewards modules, so there is no need to add this code to those templates.**

**Activate Filter**  
 This setting turns the filter on and off. It is set to “True” by default, meaning the filter is on and active.

**Sort Order of Display**  
 This setting changes the order in which the filter is displayed on the filter list.

13. When you have completed your configurations, click the “Update button”

Configuration of the Numinix Store Credit Balance Reminder module is now complete!

 

## Test & Run the Module

Navigate back to the Numinix Store Credit Balance Reminder module in the MailBeez module tab and click on it to display the function buttons on its configuration panel.

The 5 function buttons are the controls that allow you to preview your email template customizations, test the module, and then manually run it in both simulation & production mode when you’re ready:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/function_buttons.png&w=175&h=184&zc=1&q=100 "Function Buttons")](http://mailbeez.com/images/doc/common_images/function_buttons.png "Function Buttons")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Email Templates – “HTML” Button**  
 This button allows you to preview the various module templates in a nice popup window in HTML format. This way, you can easily see what the email template looks like and quickly determine which aspects of the template you’ll want to customize for your use.

As you modify your template files, you can come back and use this button to view your changes to ensure that they are appearing as you intend.

**When you’re ready to customize your email templates, have a look at our [Customizing Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)**

To view a different set of template files, go to the module’s configuration panel, click “Edit”, change your Layout Style selection, click “Update”, and return here to view them.

**Email Templates – “TXT” Button**  
 This button allows you to preview the module templates in a nice popup window in text format. Everyone has customers who prefer to receive email in text format. This tool allows you to see what they see, and preview changes you make to the template before they go out to your customers.

**Recipients – “Show” Button**  
 Clicking this button will result in a nice popup window in your admin which is populated with a list of everyone who is getting this email in the next run.

**Send Test Email – “Send” Button**  
 This button does just what it says – it lets you send a test email with test data. A really nice feature of MailBeez premium modules is that test emails include a display of the product list (if used by the module) using random products from your store. This allows you to see exactly what your customers will see – and if you enjoy experimenting with your List Engine settings, then this goes from being a nice feature to a necessary one!

**Run this module – “Run” Button**  
 This is the button you use to actually run the module. This button respects your run mode as it is set in your Simulation Configuration, so if you’re in Simulation Mode, clicking this button results in a simulation run. If you are in Production Mode, clicking this button results in a production run.

It even tells you in the text above the button which mode you’re in. This prevents you from accidentally sending emails out to customers when you’re testing.

**If you need further assistance understanding how to run simulations and send test emails, have a look at our [Testing MailBeez tutorial](/documentation/tutorials/testing-mailbeez)**



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.

## Template Manager

Mailbeez has developed a handy module that easily allows you to both edit and view your text changes right from the MailBeez interface within your store’s admin. Fully functional with all official MailBeez Modules (free, premium, and custom built), the MailBeez Template Manager makes editing a template a breeze, so much so that you may wonder how you ever lived without it! **[ Learn more!](/documentation/configbeez/config_tmplmngr/)**
