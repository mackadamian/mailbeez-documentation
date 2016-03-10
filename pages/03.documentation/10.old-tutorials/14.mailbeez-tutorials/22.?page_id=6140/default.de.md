---
# http://learn.getgrav.org/content/headers
title: Reorder Advanced with Coupons
slug: ID-6140
# menu: Reorder Advanced with Coupons
date: 14-09-2012
published: false
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

(English)

The screenshots used in this tutorial were made using Zen Cart. If you use a different e-commerce platform, your admin interface and MailBeez interface may appear slightly different, however the concepts and configuration instructions are the same across all platforms.

## About This Module

The Reorder Advanced with Coupons module lets you thank your customers for their business and reward them with a coupon for their next purchase. This helps to build customer loyalty and drive repeat business, which is crucial to the success of your company.

With 80% of your sales coming from 20% of your customer base, you can’t afford to overlook these most important customers!

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Reorder Advanced with Coupons module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/reorder_advanced/install.png&w=175&h=70&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/reorder_advanced/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/reorder_advanced/reorder_config.png&w=175&h=819&zc=1&q=100 "Reorder Advanced Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/reorder_advanced/reorder_config.png "Reorder Advanced Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configure the Review Reward Coupon Module

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/reorder_advanced/general_settings.png&w=175&h=906&zc=1&q=100 "Reorder Advanced General Settings")](http://www.mailbeez.com/images/doc/mailbeez/reorder_advanced/general_settings.png "Reorder Advanced General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Order Status, Minimum Age, Maximum Age, Order Status to Count, Number of Orders & Number of Times**  
 These 6 settings work together to identify eligible customers & create a window of time in which MailBeez will look for them when the Reorder Advanced module is run.

**Order Status Trigger**  
 This setting lets you define the order status an order must have to trigger a Reorder coupon email to be sent. By default, it is set to an order status of “Delivered”, “Completed”, or “Dispatched”, depending on your e-commerce platform. Customers who have an order status that matches this setting and who fall within the parameters defined in the remaining settings will receive a Reorder coupon email when this module is run.

**Minimum Age of Order**  
 This setting tells MailBeez to target orders “X” number of days after they reach the required order status as defined by the “Order Status Trigger” setting. By default it is set to “5”, meaning that orders which have reached the configured “Order Status” 5 or more days ago are eligible to receive a Reorder coupon email when this module is run.

**Maximum Age of Order**  
 This setting tells MailBeez to target orders “X” number of days after they reach the required order status as defined by the “Order Status Trigger” setting. By default it is set to “10”, meaning that orders which have reached the configured “Order Status” 10 or more days ago are eligible to receive a Reorder coupon email when this module is run.

The default settings of 5 days minimum and 10 days maximum tell MailBeez to target customers with orders matching the required order status within the last 5 to 10 days.

**Order Status to Count**  
 If you want to send a Reorder coupon email to only those customers who have previous orders, this setting lets you define what the status of those orders should be in order to be counted as a previous order. By default, it is set to an order status of “Delivered”, “Completed”, or “Dispatched”, depending on your e-commerce platform.

Orders matching this status will be counted as eligible previous orders.

**Number of Orders Before Sending a Reorder Coupon**  
 If you want to send a Reorder coupon email to only those customers who have previous orders, this setting lets you define how many previous orders the customer must have to be eligible to receive a Reorder coupon email.

It is set to 0 by default, meaning that customers do not need to have previous eligible orders to to receive a Reorder coupon email when this module is run.

**Number of Times to Send a Reorder Coupon**  
 This setting lets you control the maximum number of times a customer can receive a Reorder coupon email. It is set to “2″ by default, meaning that no matter how many purchases a customer makes, they will only receive a Reorder coupon email 2 times.

Using the default settings as an example, these six settings work together to tell MailBeez, “Search my database and find all customers who have received a Reorder coupon email less than 2 times and send them a Reorder coupon email”.

This is because the “Number of Orders Before Sending” setting is set to “0″, so all of the settings related to order age and order status get ignored when the module is run. Only the “Number of Times” setting is respected in this scenario.

But, if you change the “Number of Orders Before Sending” setting to “2″, for example, then these six settings work together to tell MailBeez “Search my database and find all customers who have at lest 2 orders which have reached an order status of “Delivered” within the last 5 to 10 days. Of those, filter out any customers who have already received a Reorder coupon email 2 times. Send the remaining customers a Reorder coupon email”.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Days Coupon is Valid**  
 This setting allows you define the number of days the coupon will be valid. After these number of days pass, the coupon will expire. By default, it is set to 14 days, but you may change it if you wish.

**Consider adding the [Coupon Expiry Reminder](/documentation/mailbeez/coupon_expire/) module to your MailBeez installation to increase the conversion rate of coupon emails and thereby generate more sales! Powerful!**

**Coupon Template**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

**Length of Coupon Code**  
 This setting allows you to define the length of the coupon code that MailBeez will generate. By default it is set to 8 characters. You may change it if you wish, keeping in mind that the longer the code, the more character combinations are possible. If you make this code too short, you could limit the number of available character combinations, thereby limiting the number of unique coupon codes that MailBeez can generate.

**Layout**  
 This setting allows you to choose which layout style template set you want to assign & use for this module.

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

**Random Products for Testing**  
 MailBeez Premium modules display actual product lists in your test emails, enabling you to see what the product list looks like in the various layout style templates. Additionally, if you utilize the List Engine configuration settings to change the layout and appearance of your product lists in your email templates, this feature will allow you to preview those changes in test emails prior to you sending the emails to your customers.

The configuration setting is already pre-populated with random product id’s from your store, but you may change them if you wish to use specific products in your testing.

Once you’ve completed your configurations, click the “Update” button.

 

## Coupon Engine, List Engine & Social Sharing

The Reorder Advanced with Coupons module adds three new configuration groups to your MailBeez installation: Coupon Engine configuration, List Engine configuration, and Social Sharing configuration.

All three are common configuration groups shared by multiple premium email modules. If you have already configured them after installing another module, you may skip these steps.

Otherwise:

1. Navigate to the Configuration tab of the MailBeez interface:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/config_tab3.png&w=270&h=174&zc=1&q=100 "MailBeez Configuration Tab")](http://mailbeez.com/images/doc/common_images/config_tab3.png "MailBeez Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Locate and click on ‘Coupon Engine’ to bring up the Coupon Engine configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/coupon_engine_config.png&w=175&h=154&zc=1&q=100 "Coupon Engine Configuration Panel")](http://mailbeez.com/images/doc/common_images/coupon_engine_config.png "Coupon Engine Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. As you can see from the image above, there are no actual settings here to configure, but you need to be aware of this configuration option because it allows you to delete all simulation coupons. When you run simulations, MailBeez will create simulated coupon codes which are unnecessary once simulations are complete. Once you’ve completed all your simulated runs of this module, return here and click on the “Delete” button to delete the simulation coupons.
6. Locate and click on ‘List Engine’ to bring up the List Engine configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/list_engine_configuration.png&w=175&h=229&zc=1&q=100 "List Engine Configuration Settings")](http://mailbeez.com/images/doc/common_images/list_engine_configuration.png "List Engine Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The List Engine settings allow you to configure the layout and appearance of the product list in the emails generated by the modules that include product lists in the email content.

**Column Layout – Number of Columns**  
 This setting allows you to configure the number of columns you wish to display for multi-column product list layouts. The number you enter here must be supported by the list sub-template used by the layout setting templates you selected to use for this module. By default, this is set to 3 columns.

**Limit Number of Listed Products**  
 This setting allows you to place a limit on how many products are displayed in the emails generated by the modules that include product lists in the email content.

**Both of these settings may be overridden by modules or sub-templates.**

12. When you’ve completed your configurations, click the “Update” button
13. Locate and click on ‘Social Sharing Services’ to bring up the Social Sharing configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/social_sharing_config.png&w=175&h=101&zc=1&q=100 "Social Sharing Configuration Settings")](http://mailbeez.com/images/doc/common_images/social_sharing_config.png "Social Sharing Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The Social Sharing setting allows you to control which social sharing applications you want to display beneath each product of the product listing in the emails generated by the modules that include product lists in the email content.

By default, all three available options are selected.

17. When you’ve completed your configurations, click the “Update” button

 

## Install & Configure the Layout Optimizer Filter

The Reorder Advanced with Coupons module adds a new filter to your MailBeez installation: the Layout Optimizer filter.

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

Configuration of the Reorder Advanced with Coupons module is now complete!

 

## Create & Assign Coupon Templates

Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return to the module to assign a coupon template to each email cycle using the drop down box in each email cycle’s configuration panel (see the section of the tutorial on configuring email cycles).

Once you’ve done that, it’s time to test & run some simulations.

 

## Test & Run the Module

Navigate back to the Reorder Advanced with Coupons module in the MailBeez module tab and click on it to display the function buttons on its configuration panel.

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
