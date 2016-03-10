---
# http://learn.getgrav.org/content/headers
title: Birthday Greetings Coupon
slug: ID-5745
# menu: Birthday Greetings Coupon
date: 30-08-2012
published: false
publish_date: 30-08-2012
# unpublish_date: 30-08-2012
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

(English)

The screenshots used in this tutorial were made using Zen Cart. If you use a different e-commerce platform, your admin interface and MailBeez interface may appear slightly different, however the concepts and configuration instructions are the same across all platforms.

## About This Module

The Birthday Greetings Coupon module takes advantage of Mailbeez’s intelligent architecture by providing your store with the ability to send an individual, personalized coupon to each customer to let them know you are thinking about them during their special day.

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Birthday Greetings Coupon module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_birthday/install.png&w=175&h=85&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/coupon_birthday/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_birthday/birthday_config.png&w=175&h=706&zc=1&q=100 "Birthday Greetings Coupon Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/coupon_birthday/birthday_config.png "Birthday Greetings Coupon Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configure the Birthday Greetings Coupon Module

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_birthday/general_settings.png&w=175&h=487&zc=1&q=100 "Birthday Greetings Coupon General Settings")](http://www.mailbeez.com/images/doc/mailbeez/coupon_birthday/general_settings.png "Birthday Greetings Coupon General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Target Days Before & Target Days After**  
 These settings work together to create a window of time in which MailBeez will look for opportunities to send the Birthday Greetings email by targeting customers who fall within the time frame you define with these settings.

**Target Days Before**  
 This setting lets you target customers “X” number of days before their birthday. It is set to “1” by default, meaning that when this module is run, MailBeez will target customers who have a birthday 1 day in the future.

If you want customers to receive the Birthday Greetings emails more than 1 day ahead of their birthday, change this setting to a higher number.

**Target Days After**  
 This setting lets you target customers who had a birthday “X” number of days ago. By default it is set to “2”, meaning that when this module is run, MailBeez will target all customers who had a birthday within the past 2 days.

The default settings of 1 day before and 2 days after creates a 4 day window of time (1 day before + today + 2 days after = 4 days). When the module is run with these settings, MailBeez will find and send an email to all customers who have a birthday falling within that window and who have not yet received the Birthday Greetings Coupon email.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Coupon Template**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

**Days Coupon is Valid**  
 This setting allows you define the number of days the coupon will be valid. After these number of days pass, the coupon will expire. By default, it is set to 14 days, but you may change it if you wish.

**Consider adding the [Coupon Expiry Reminder](/documentation/mailbeez/coupon_expire/) module to your MailBeez installation to increase the conversion rate of coupon emails and thereby generate more sales! Powerful!**

**Length of Coupon Code**  
 This setting allows you to define the length of the coupon code that MailBeez will generate. By default it is set to 8 characters. You may change it if you wish, keeping in mind that the longer the code, the more character combinations are possible. If you make this code too short, you could limit the number of available character combinations, thereby limiting the number of unique coupon codes that MailBeez can generate.

**Layout**  
 This setting allows you to choose which layout style template set you want to assign & use for this module.

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

Once you’ve completed your configurations, click the “Update” button.

 

## The Coupon Engine

The Birthday Greetings Coupon module adds a new configuration group to your MailBeez installation: Coupon Engine configuration. This is a common configuration group shared by multiple premium email modules. If you have already configured this group after installing another module, you may skip these steps.

Otherwise:

1. Navigate to the Configuration tab of the MailBeez interface:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/config_tab3.png&w=270&h=174&zc=1&q=100 "MailBeez Configuration Tab")](http://mailbeez.com/images/doc/common_images/config_tab3.png "MailBeez Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Locate and click on ‘Coupon Engine’ to bring up the Coupon Engine configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/coupon_engine_config.png&w=175&h=154&zc=1&q=100 "Coupon Engine Configuration Panel")](http://mailbeez.com/images/doc/common_images/coupon_engine_config.png "Coupon Engine Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. As you can see from the image above, there are no actual settings here to configure, but you need to be aware of this configuration option because it allows you to delete all simulation coupons. When you run simulations, MailBeez will create simulated coupon codes which are unnecessary once simulations are complete. Once you’ve completed all your simulated runs of this module, return here and click on the “Delete” button to delete the simulation coupons.

 

## Install & Configure the Layout Optimizer Filter

The Birthday Greetings Coupon module adds a new filter to your MailBeez installation: the Layout Optimizer filter.

The Layout Optimizer filter optimizes the presentation of your emails by fixing tables, removing html comments, wrapping lines of text and removing excess whitespaces.

This is a common filter shared by multiple premium email modules, so if you’ve already installed & configured this filter, you may skip these steps. Otherwise:

1. Click on the Layout Optimizer filter and then click its ‘Install’ button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/layout_optimizer_install.png&w=175&h=70&zc=1&q=100 "Install Layout Filter")](http://mailbeez.com/images/doc/common_images/layout_optimizer_install.png "Install Layout Filter")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click on the “Edit” button to bring up the filter’s configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/layout_optimizer_config.png&w=175&h=267&zc=1&q=100 "Layout Filter Configuration Settings")](http://mailbeez.com/images/doc/common_images/layout_optimizer_config.png "Layout Filter Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. It is recommended that you leave these settings as they are unless you have a need to change them:
**Activate Filter**  
 This setting turns the filter on and off. It is set to “True” by default, meaning the filter is on and active.

**Fix Table**  
 This setting allows you to enable MailBeez’s ability to fix table structure in the email templates for best output results.

**Remove HTML Comments**  
 The premium layouts contain comments for easier editing. This setting allows for the removal of these empty HTML comments from your email template code.

**Wrap Lines to 76 Characters**  
 This setting enables the forcing of text lines in email templates to wrap at 76 characters whenever possible in order to protect the integrity of the templates design.

**Remove Excess Whitespace**  
 This setting allows you to enable MailBeez to remove excess whitespace from your email templates in order to keep the design nice and tight and reduce the size of the email.

11. When you have completed your configurations, click the “Update button”

Configuration of the Birthday Greetings Coupon module is now complete!

 

## Create & Assign Coupon Templates

Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return to the module to assign a coupon template to each email cycle using the drop down box in each email cycle’s configuration panel (see the section of the tutorial on configuring email cycles).

Once you’ve done that, it’s time to test & run some simulations.

 

## Test & Run the Module

Navigate back to the Birthday Greetings Coupon module in the MailBeez module tab and click on it to display the function buttons on its configuration panel.

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
