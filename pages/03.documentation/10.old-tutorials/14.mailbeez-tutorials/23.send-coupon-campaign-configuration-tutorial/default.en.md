---
# http://learn.getgrav.org/content/headers
title: Send Coupon Campaign
slug: send-coupon-campaign-configuration-tutorial
# menu: Send Coupon Campaign
date: 14-09-2012
published: true
publish_date: 14-09-2012
# unpublish_date: 14-09-2012
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

The Send Coupon Campaign Module lets you create & manage specific coupon campaigns. It’s perfect for holiday, special occasion, seasonal campaigns, or any time you wish to send a coupon campaign in bulk!

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

**Important:** If you want to sent a different campaign, you need to create and configure a different template coupon! The System tracks which customer has received which coupon and will not sent the new campaign unless you have assigned a new template coupon

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Locate the Send Coupon Campaign module and click on it.
2. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_campaign/install.png&w=175&h=77&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/coupon_campaign/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_campaign/coupon_campaign_config.png&w=175&h=818&zc=1&q=100 "Send Coupon Campaign Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/coupon_campaign/coupon_campaign_config.png "Send Coupon Campaign Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

## Configure the Coupon Campaign Module

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_campaign/general_settings.png&w=175&h=789&zc=1&q=100 "Send Coupon Campaign General Settings")](http://www.mailbeez.com/images/doc/mailbeez/coupon_campaign/general_settings.png "Send Coupon Campaign General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Start Date, End Date, Target Order Status, Age of Last Order & Days to Look Back**  
 These 5 settings work together to identify eligible customers & create a window of time in which MailBeez will look for them when the Coupon Campaign module is run.

**Start Date of Campaign**  
 This field is blank, allowing you to enter the date you want your Coupon Campaign to begin. If you have MailBeez configured to run automatically, the bulk sending of the current campaign will begin on the next run following the start date.

Before the campaign run begins, the module will appear as if it is in an inactive status. This is normal. Always leave the “Activate Module” status set to “True” unless you want to disable the module.

**End Date of Campaign**  
 This field is blank, allowing you to enter the date you want your Coupon Campaign to end. Once the campaign run ends, the module will once again appear as if it is in an inactive status. This is normal. Always leave the “Activate Module” status set to “True” unless you want to disable the module.

**Target Order Status**  
 This setting lets you define which order status the customer’s last order must have to receive a Coupon Campaign email. By default, it is set to an order status of “Delivered”, “Completed”, or “Dispatched”, depending on your e-commerce platform. Customers whose last order has an order status that matches this setting and who fall within the parameters defined in the remaining settings will receive a Coupon Campaign email when this module is run.

**Age of Last Order**  
 This setting lets you define how many days old the customer’s last order must be to be eligible to receive a Coupon Campaign email. By default it is blank, meaning that customers with orders which have reached the configured “Order Status” are eligible to receive a Coupon Campaign email when this module is run, regardless of the age of their last order.

**Days to Look Back**  
 This setting lets you define how far back in time MailBeez should look to find customers who have an order that meets the “Age of Last Order” criteria. By default, it is blank, meaning that customers with orders which have reached the configured “Order Status” are eligible to receive a Coupon Campaign email when this module is run, regardless of the age of their last order.

**Coupon Template**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

**Days Coupon is Valid**  
 This setting allows you define the number of days the coupon will be valid. After these number of days pass, the coupon will expire. By default, it is set to 14 days, but you may change it if you wish.

**Consider adding the [Coupon Expiry Reminder](/documentation/mailbeez/coupon_expire/) module to your MailBeez installation to increase the conversion rate of coupon emails and thereby generate more sales! Powerful!**

**Length of Coupon Code**  
 This setting allows you to define the length of the coupon code that MailBeez will generate. By default it is set to 8 characters. You may change it if you wish, keeping in mind that the longer the code, the more character combinations are possible. If you make this code too short, you could limit the number of available character combinations, thereby limiting the number of unique coupon codes that MailBeez can generate.

**Limit Number of Emails per Run**  
 Most web hosts place limits on how many emails you can send out per hour. Check with your host to find out if this is true for you. If it is, you will need to place a limit on how many emails this module sends per hour.

There are two ways to do this. You can either add the [Simple Throttling module](/documentation/filterbeez/filter_do_throttling_simple/) to your MailBeez installation, or you can use this setting to define how many emails this module should send per hour, based on your web host limitations. Then, you will need to run this module every hour until all of the emails have been sent.

By default, this setting is 1000, but again you should check with your web host and configure this setting accordingly.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Layout**  
 This setting allows you to choose which layout style template set you want to assign & use for this module.

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

Once you’ve completed your configurations, click the “Update” button.

## The Coupon Engine

The Send Coupon Campaign module adds a new configuration group to your MailBeez installation: the Coupon Engine configuration. This is a common configuration group shared by multiple premium email modules. If you have already configured this group after installing another module, you may skip these steps.

Otherwise:

1. Navigate to the Configuration tab of the MailBeez interface:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/config_tab3.png&w=270&h=174&zc=1&q=100 "MailBeez Configuration Tab")](http://mailbeez.com/images/doc/common_images/config_tab3.png "MailBeez Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Locate and click on ‘Coupon Engine’ to bring up the Coupon Engine configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/coupon_engine_config.png&w=175&h=154&zc=1&q=100 "Coupon Engine Configuration Panel")](http://mailbeez.com/images/doc/common_images/coupon_engine_config.png "Coupon Engine Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. As you can see from the image above, there are no actual settings here to configure, but you need to be aware of this configuration option because it allows you to delete all simulation coupons. When you run simulations, MailBeez will create simulated coupon codes which are unnecessary once simulations are complete. Once you’ve completed all your simulated runs of this module, return here and click on the “Delete” button to delete the simulation coupons.

## Install & Configure the Layout Optimizer Filter

The Send Coupon Campaign module adds a new filter to your MailBeez installation: the Layout Optimizer filter.

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

Configuration of the Send Coupon Campaign module is now complete!

## Create & Assign Coupon Templates

Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return to the module to assign a coupon template to each email cycle using the drop down box in each email cycle’s configuration panel (see the section of the tutorial on configuring email cycles).

Once you’ve done that, it’s time to test & run some simulations.

## Test & Run the Module

Navigate back to the Send Coupon Campaign module in the MailBeez module tab and click on it to display the function buttons on its configuration panel.

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
