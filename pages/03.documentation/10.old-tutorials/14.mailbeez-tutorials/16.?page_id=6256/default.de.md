---
# http://learn.getgrav.org/content/headers
title: Payment: Invoice Dunning
slug: ID-6256
# menu: Payment: Invoice Dunning
date: 21-09-2012
published: false
publish_date: 21-09-2012
# unpublish_date: 21-09-2012
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

An intelligent and fully automated payment reminder system, the Invoice Dunning module can be configured to send emails to all open invoice orders that are awaiting payment. Multi-step emails begin with friendly reminders and continue all the way through to debt collection.

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

### Prepare Payment Module & Create New Order Statuses

To use the Invoice Dunning module, your store must have a matching payment module in place and 2 new order statuses created. An invoice payment module should allow you to process & ship orders without payment and then bill your customer by invoice. With this in mind, follow these simple steps to prepare your store to use the Invoice Dunning Module:

1. Install an invoice payment module if you don’t already have one in place.
2. Navigate to your store’s order status area and create a new order status which indicates an open unpaid invoice, perhaps “Open Invoice Payment Due” for example. If you need assistance with this step, please see your e-commerce platform’s documentation.
3. Set the new order status as the default order status in your invoice payment module. If you need assistance with this step, please see your invoice payment module’s documentation.
4. Navigate to your store’s order status area and create a new order status for debt collection, perhaps “Debt Collection” or “In Collections” for example.

Your preparations are now complete. Information on utilizing your new order statuses with the Invoice Dunning module can be found in the configuration section of this tutorial.

### Install Configuration Settings Into Your Database

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Payment Invoice Dunning module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/install.png&w=175&h=79&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/invoice_config.png&w=175&h=411&zc=1&q=100 "Payment Invoice Dunning Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/invoice_config.png "Payment Invoice Dunning Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring Payment Invoice Dunning

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/general_settings.png&w=175&h=537&zc=1&q=100 "Payment Invoice Dunning General Settings")](http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/general_settings.png "Payment Invoice Dunning General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Order Status & Number of Days to to Look Back**  
 These settings work together to identify eligible customers & create a window of time in which MailBeez will look for them when the Payment Invoice Dunning module is run.

**Order Status for Invoice Payment Due**  
 This setting lets you define the order status an order must have to be identified by MailBeez as having an outstanding balance. The new order statuses you created in the first step of this tutorial should appear on this list. Select the order status you created as the default status for your invoice payment module. For example, “Open Invoice Payment Due”.

**Order Status for Debt Collection**  
 This setting allows the module to automatically move orders for which no payment has been received after the configured number of days into a debt-collection status. By default, this is set to an order status of “Delivered”, “Completed”, or “Dispatched”, depending on your e-commerce platform. However, you will need to change it to the new debt collection order status you created in the first step of this tutorial: “Debt Collection” or “In Collections”, for example.

**Number of Days to Look Back**  
 This setting lets you define how far back in time MailBeez should look for customers who meet the Order Status criteria when the module is run. By default, it is set to 3, meaning that MailBeez will look for eligible orders that occurred in the last three days.

These settings work together to tell MailBeez: “When this module is run, search my database for the last 3 days and find all customers who have an order status of (for example) “Open Invoice” and (for example) “In Collections”, and send out the appropriate email.

For customers with an open invoice, the “appropriate email” is one of the multi-step Demand for Payment emails, depending on where they’re at in the email cycle. For customers with a Debt Collection status, the “appropriate email” is the Debt Collection Order Notification email. See the sections below on configuring email cycles for more information.

**Debt Collection Order Notification Email**  
 When MailBeez moves a customer’s order into a debt collection status, an email is sent to the person in charge of handling collections for your business. By default, it is set to send to you using the default email address configured in your e-commerce platform’s email settings.

If you manage your own collections, you may leave this as it is or change it as you prefer. For example, perhaps you have a specific email address for debt collection. If someone else manages your debt collection for you, you may wish to enter their email address here instead of your own.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Layout**  
 This setting allows you to choose which layout style template set you want to assign & use for this module.

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

**Random Products for Testing**  
 MailBeez Premium modules display actual product lists in your test emails, enabling you to see what the product list looks like in the various layout style templates. Additionally, if you utilize the List Engine configuration settings to change the layout and appearance of your product lists in your email templates, this feature will allow you to preview those changes in test emails prior to you sending the emails to your customers.

The configuration setting is already pre-populated with random product id’s from your store, but you may change them if you wish to use specific products in your testing.

Once you’ve completed your configurations, click the “Update” button.

### Configure the Friendly Payment Demand Notice Email Cycle

Once you’ve finished configuring the module’s general settings, you need to configure the settings for each email cycle:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/email_cycles.png&w=270&h=83&zc=1&q=100 "Invoice Dunning Email Cycles")](http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/email_cycles.png "Invoice Dunning Email Cycles")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Click on the Friendly Payment Demand Notice email cycle beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/1st_email_config.png&w=175&h=83&zc=1&q=100 "Friendly Payment Demand Notice Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/1st_email_config.png "Friendly Payment Demand Notice Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Number of Days to Delay for Step 1**  
 If your invoice payment module and custom order status are set up correctly, an order should reach the configured “Invoice Payment Due Order Status” as soon as it is placed.

Therefore, another way to look at this setting is to ask “How many days after an order is placed should MailBeez wait to send the Friendly Payment Demand Notice 1 email?

By default this is set to 3, meaning that any order which is 3 days old and has a balance due will receive this email when the module is run.

Whatever you enter here will display next to its email cycle on the MailBeez Modules tab, so you can always see, at a glance, what your setting is.

### Configure the Payment Demand Notice II Email Cycle

1. Click on the Payment Demand Notice II email cycle beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/2nd_email_config.png&w=175&h=83&zc=1&q=100 "Payment Demand Notice II Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/2nd_email_config.png "Payment Demand Notice II Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Number of Days to Delay for Step 2**  
 How many days after the Friendly Payment Demand Notice email is sent should MailBeez wait to send the Payment Demand Notice II email? By default, it is set to 2, meaning that any order which is 5 days old and has a balance due will receive this email when the module is run.

Whatever number you enter here will be added to the number you entered for the Step 1 Delay to get the total number of days since the order was placed. This total will then display next to its email cycle on the MailBeez Modules tab. This allows you to easily see how old the order must be for the Payment Demand Notice II email to be sent.

### Configure the Final Payment Demand Notice Email Cycle

1. Click on the Final Payment Demand Notice email cycle beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/3rd_email_config.png&w=175&h=83&zc=1&q=100 "Final Payment Demand Notice Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/3rd_email_config.png "Final Payment Demand Notice Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Number of Days to Delay for Step 3**  
 How many days after the Payment Demand Notice II email is sent should MailBeez wait to send the Final Payment Demand Notice email? By default, it is set to 2, meaning that any order which is 7 days old and has a balance due will receive this email when the module is run.

Whatever number you enter here will be added to the numbers you entered for the Step 1 & Step 2 Delay settings to get the total number of days since the order was placed. This total will then display next to its email cycle on the MailBeez Modules tab. This allows you to easily see how old the order must be for the Final Payment Demand Notice email to be sent.

### Configure the Debt Collection Email Cycle

When this module is run, MailBeez will take any order that is the configured number of days old and change its status to the configured order status for debt collection, and then send this Debt Collection email to the customer(s).

1. Click on the Debt Collection email cycle beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/4th_email_config.png&w=175&h=91&zc=1&q=100 "Debt Collection Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/4th_email_config.png "Debt Collection Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Number of Days to Delay for Step 4**  
 How many days after the Final Payment Demand Notice email is sent should MailBeez wait to send the Debt Collection email? By default, it is set to 1, meaning that any order which is 8 days old and has a balance due will receive this email when the module is run.

Whatever number you enter here will be added to the numbers you entered for the Step 1, Step 2, and Step 3 Delay settings to get the total number of days since the order was placed. This total will then display next to its email cycle on the MailBeez Modules tab. This allows you to easily see how old the order must be for the Debt Collection email to be sent.

### Configure the Debt Collection Case Notification Email Cycle

1. Click on the Debt Collection Case Notification email cycle beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/5th_email_config.png&w=175&h=124&zc=1&q=100 "Debt Collection Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/payment_invoice_dunning/5th_email_config.png "Debt Collection Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Number of Days to Delay for Step 5**  
 How many days after the Debt Collection email is sent should MailBeez wait to send the Debt Collection Case Notification email? By default, it is set to 0, meaning that any order which is 8 days old and has a balance due will receive this email when the module is run.

In other words, this setting will result in both you and your customer being notified of the debt collection status on the same day.

Whatever number you enter here will be added to the numbers you entered for the Step 1, Step 2, Step 3, and Step 4 Delay settings to get the total number of days since the order was placed. This total will then display next to its email cycle on the MailBeez Modules tab. This allows you to easily see how old the order must be for the Debt Collection Case Notification email to be sent.

 

## Configure List Engine & Social Sharing Settings

The Payment Invoice Dunning module adds two new configuration groups to your MailBeez installation: List Engine configuration and Social Sharing configuration.

These are common configuration groups shared by multiple premium email modules. If you have already configured them after installing another module, you may skip these steps.

Otherwise:

1. Navigate to the Configuration tab of the MailBeez interface:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/config_tab3.png&w=270&h=174&zc=1&q=100 "MailBeez Configuration Tab")](http://mailbeez.com/images/doc/common_images/config_tab3.png "MailBeez Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Locate and click on ‘List Engine’ to bring up the List Engine configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/list_engine_configuration.png&w=175&h=229&zc=1&q=100 "List Engine Configuration Settings")](http://mailbeez.com/images/doc/common_images/list_engine_configuration.png "List Engine Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The List Engine settings allow you to configure the layout and appearance of the product list in the emails generated by the modules that include product lists in the email content.

**Column Layout – Number of Columns**  
 This setting allows you to configure the number of columns you wish to display for multi-column product list layouts. The number you enter here must be supported by the list sub-template used by the layout setting templates you selected to use for this module. By default, this is set to 3 columns.

**Limit Number of Listed Products**  
 This setting allows you to place a limit on how many products are displayed in the emails generated by the modules that include product lists in the email content.

**Both of these settings may be overridden by modules or sub-templates.**

9. When you’ve completed your configurations, click the “Update” button
10. Locate and click on ‘Social Sharing Services’ to bring up the Social Sharing configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/social_sharing_config.png&w=175&h=101&zc=1&q=100 "Social Sharing Configuration Settings")](http://mailbeez.com/images/doc/common_images/social_sharing_config.png "Social Sharing Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The Social Sharing setting allows you to control which social sharing applications you want to display beneath each product of the product listing in the emails generated by the modules that include product lists in the email content.

By default, all three available options are selected.

14. When you’ve completed your configurations, click the “Update” button

 

## Install & Configure Additional Filters

The Payment Invoice Dunning module adds a new filter to your MailBeez installation: the Layout Optimizer filter.

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

Configuration of the module is now complete!

 

## Test & Run the Payment Invoice Dunning Module

Now that you’ve completed configuration of your module, it’s time to test!

1. Navigate back to the Payment Invoice Dunning module in the MailBeez module tab.
2. Click it to display the module’s email cycle options.
3. Each email cycle option’s configuration panel features the same set of function buttons. These should look familiar because they are the same buttons found in all of the email modules.

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
