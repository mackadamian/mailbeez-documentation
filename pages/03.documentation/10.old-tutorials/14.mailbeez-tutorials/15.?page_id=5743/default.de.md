---
# http://learn.getgrav.org/content/headers
title: Nopurchase Advanced
slug: ID-5743
# menu: Nopurchase Advanced
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

This highly useful eCommerce email add-on gives you the tools to automatically email customers who created an account, but did not purchase from your store, at the same time offering them a personalized discount coupon to tempt them into making their first purchase.

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Nopurchase Advanced module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/install.png&w=175&h=85&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/nopurchase_config_panel.png&w=175&h=429&zc=1&q=100 "Nopurchase Advanced Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/nopurchase_config_panel.png "Nopurchase Advanced Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring Nopurchase Advanced

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/general_settings_panel.png&w=175&h=582&zc=1&q=100 "Nopurchase Advanced General Settings")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/general_settings_panel.png "Nopurchase Advanced General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Workflow – Number of Nopurchase Emails (1-4+)**  
 This setting lets you control how many Nopurchase email cycles you want the module to complete for each customer meeting the criteria to receive Nopurchase emails. By default, this setting is set to Loop but you may decrease it if you wish.

The number you select here also controls which email cycle options are displayed beneath the module name in the MailBeez Modules tab & are therefore available for configuration, testing, and use. Images of this concept are below.

**For each email cycle, MailBeez will disregard customers who have already received a Nopurchase email from that cycle, ensuring that a customer will not receive the same email from the same cycle more than once. **

**Send 1 Email**  
 Setting this to 1 will result in only the ‘First Nopurchase’ email cycle option being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/email_cycle1.png&w=270&h=45&zc=1&q=100 "Nopurchase Advanced Email Cycle Option 1")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/email_cycle1.png "Nopurchase Advanced Email Cycle Option 1")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive only one email enticing them back to your store. If they fail to use the enclosed link to return to the store and make a purchase, they will not be emailed again.

**Send 2 Emails**  
 Setting this to 2 will result in the ‘First Nopurchase’ and ‘Second Nopurchase’ email cycle options being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/email_cycle2.png&w=270&h=53&zc=1&q=100 "Nopurchase Advanced Email Cycle Option 2")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/email_cycle2.png "Nopurchase Advanced Email Cycle Option 2")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive the First Nopurchase email enticing them back to your store. If they fail to use the enclosed link to return to the store and make a purchase, they will receive the Second Nopurchase email “X” number of days later, based on your configuration settings. More on this configuration setting later.

**Send 3 Emails**  
 Setting this to 3 will result in the ‘First Nopurchase’, ‘Second Nopurchase’, and ‘Third Nopurchase’ email cycle options being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/email_cycle3.png&w=270&h=59&zc=1&q=100 "Nopurchase Advanced Email Cycle Option 3")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/email_cycle3.png "Nopurchase Advanced Email Cycle Option 3")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive the First Nopurchase email enticing them back to your store. If they fail to use the enclosed link to return to the store and make a purchase, they will receive the Second Nopurchase email “X” number of days later, based on your configuration settings. If the customer again fails to use the enclosed link to return to the store and make a purchase, the Third Nopurchase email will be sent “X” number of days later, based on your configuration settings. More on this configuration setting later.

**Send Loop Emails**  
 Setting this to Loop will result in the ‘First Nopurchase’, ‘Second Nopurchase’, ‘Third Nopurchase’, and ‘Nopurchase Loop’ email cycle options being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/email_cycle4.png&w=270&h=66&zc=1&q=100 "Nopurchase Advanced Email Cycle Option Loop")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/email_cycle4.png "Nopurchase Advanced Email Cycle Option Loop")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive the First Nopurchase email enticing them back to your store. If they fail to use the enclosed link to return to the store and make a purchase, they will receive the Second Nopurchase email “X” number of days later, based on your configuration settings. If the customer again fails to use the enclosed link to return to the store and make a purchase, the Third Nopurchase email will be sent “X” number of days later, based on your configuration settings.

If the customer still fails to use the enclosed link to return to the store and make a purchase, they will begin to receive Nopurchase emails in an ongoing loop as often as you configure the loop to continue. More on this configuration setting later.

Be careful with this setting. If you decide to use the loop option, you’ll want to avoid being flagged by your old customers as a spammer – or worse – reported by your customers to potential customers via social media.

One good way to avoid this is to create a variety of templates and offerings for the loop iteration and change them out between runs of the module. This ensures that customers are always receiving fresh content. To them, it looks like a newsletter, whereas sending the same content and same offer over and over again just looks like spam.

**Check For Empty Customer Basket**  
 This setting allows you to tell MailBeez to check the customer’s shopping cart for contents, and then send a Nopurchase email only when the shopping cart is empty. By default, it is set to “False”, meaning that Nopurchase emails will be sent to eligible customers regardless of the status of their shopping cart.

**Target Days Without Purchase & Target Days to to Look Back**  
 These 2 settings work together to identify eligible customers & create a window of time in which MailBeez will look for them when the Nopurchase Advanced module is run.

**Target Days Without Purchase**  
 This setting lets you target customers who have created an account but have not made a purchase after “X” number of days. By default it it set to 2, meaning that if a customer creates an account and still has not made a purchase 2 days later, MailBeez will target them for a Nopurchase email when the Nopurchase module is run.

If you want to give your customers more time to make a purchase before sending out the Nopurchase email, simply increase this number. Conversely, if you want to give them less time without a purchase before contacting them, you will lower this number.

**Target Days to Look Back**  
 This setting lets you define how far back in time MailBeez should look for customers who meet the Days Without Purchase criteria. By default, it is set to 10 and must always be a higher number than the “Target Days Without Purchase” setting.

The default settings of 2 Days Without Purchase and 10 Days to Look Back work together to tell MailBeez “Search my database for the last 10 days and find all customer accounts that were created but show no purchases made after 2 days, and send them a Nopurchase email.”

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

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

### Configure the First Nopurchase Email Cycle

1. Click on the First Nopurchase email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/1st_email_config.png&w=175&h=176&zc=1&q=100 "First Nopurchase Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/1st_email_config.png "First Nopurchase Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Target Days Without Purchase**  
 This setting is identical to its counterpart in the module’s general configuration settings and is placed here for convenience. Changing the setting in this panel will automatically update it the module’s general configurations panel. The converse is also true; changing the setting in the module’s general configurations panel will update the setting here in this panel.

Whatever you enter here will display next to the First Nopurchase email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your setting is. Handy!

**Coupon Template – First Nopurchase Email**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

### Configure the Second Nopurchase Email Cycle

1. Click on the Second Nopurchase email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/2nd_email_config.png&w=175&h=184&zc=1&q=100 "Second Nopurchase Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/2nd_email_config.png "Second Nopurchase Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Second Nopurchase Email Delay**  
 This setting allows you to tell MailBeez how many days to wait after sending out the First Nopurchase email before sending out the Second Nopurchase email. By default, it it set to 2, but you should probably increase it slightly. Since each email cycle will ideally contain better and better coupon offers, sending out Nopurchase emails too close together can train your customers to wait for the best offer and possibly cheapen your business reputation.

Whatever you enter here will display next to the Second Nopurchase email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your setting is. Handy!

**Coupon Template – Second Nopurchase Email**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

### Configure the Third Nopurchase Email Cycle

1. Click on the Third Nopurchase email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/3rd_email_config.png&w=175&h=183&zc=1&q=100 "Third Nopurchase Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/3rd_email_config.png "Third Nopurchase Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Third Nopurchase Email Delay**  
 This setting allows you to tell MailBeez how many days to wait after sending out the Second Nopurchase email before sending out the Third Nopurchase email. By default, it it set to 5.

Whatever you enter here will display next to the Third Nopurchase email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your setting is. Handy!

**Coupon Template – Third Nopurchase Email**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

### Configure the Nopurchase Loop Email Cycle

1. Click on the Nopurchase Email Loop email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/4th_email_config.png&w=175&h=218&zc=1&q=100 "Loop Nopurchase Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/4th_email_config.png "Loop Nopurchase Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Nopurchase Email Loop Delay**  
 This setting allows you to tell MailBeez how many days to wait after sending out the Third Nopurchase email before starting the Nopurchase Email Loop. By default, it it set to 10.

**Nopurchase Loop Period**  
 This setting allows you to tell MailBeez how often, in days, to repeat the Nopurchase email loop. By default, it is set to 15.

Whatever you enter for these two settings will display next to the Nopurchase Email Loop email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your settings are. Handy!

**Coupon Template – Loop**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

 

## The Coupon Engine

The Nopurchase Advanced module adds a new configuration group to your MailBeez installation: Coupon Engine configuration. This is a common configuration group shared by multiple premium email modules. If you have already configured this group after installing another module, you may skip these steps.

Otherwise:

1. Navigate to the Configuration tab of the MailBeez interface:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/config_tab3.png&w=270&h=174&zc=1&q=100 "MailBeez Configuration Tab")](http://mailbeez.com/images/doc/common_images/config_tab3.png "MailBeez Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Locate and click on ‘Coupon Engine’ to bring up the Coupon Engine configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/coupon_engine_config.png&w=175&h=154&zc=1&q=100 "Coupon Engine Configuration Panel")](http://mailbeez.com/images/doc/common_images/coupon_engine_config.png "Coupon Engine Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. As you can see from the image above, there are no actual settings here to configure, but you need to be aware of this configuration option because it allows you to delete all simulation coupons. When you run simulations, MailBeez will create simulated coupon codes which are unnecessary once simulations are complete. Once you’ve completed all your simulated runs of this module, return here and click on the “Delete” button to delete the simulation coupons.

 

## Install & Configure Additional Filters

The Nopurchase Advanced module adds two new filters to your MailBeez installation: the Check Nopurchase filter and the Layout Optimizer filter.

1. Navigate to filter & helper tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/filter_tab2.png&w=270&h=68&zc=1&q=100 "MailBeez Filter & Helper Tab")](http://www.mailbeez.com/images/doc/common_images/filter_tab2.png "MailBeez Filter & Helper Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click on the Check Nopurchase filter and then click its ‘Install’ button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/nopurchase_check_filter_install.png&w=175&h=84&zc=1&q=100 "Install Nopurchase Check Filter")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/nopurchase_check_filter_install.png "Install Nopurchase Check Filter")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. Click on the “Edit” button to bring up the filter’s configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/nopurchase_check_filter_config.png&w=175&h=81&zc=1&q=100 "Nopurchase Check Filter Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/nopurchase_check_filter_config.png "Nopurchase Check Filter Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

As you can see from the image above, there is only one configuration setting here – activate or deactivate the filter. It is set to “True” by default, meaning the filter is active.

However, the Check Nopurchase filter is only necessary if you were running the Nopurchase Simple module prior to installing the advanced module. It’s function is to prevent the advanced module from resending to clients already contacted by simple module. It also checks to see if customers have blocked the simple module, and if so, blocks them from receiving the advanced module mailings.

9. If you were not using the Nopurchase Simple module, change this setting to “False” to disable it.
10. When you have completed your configurations, click the “Update” button

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

 

## Install & Configure Coupon Dashboard Widget

The Nopurchase Advanced module adds a new dashboard widget to your MailBeez installation: the Search Coupon Dashboard Widget. This widget allows you to search for any coupon by coupon code, coupon name, or parts of a code or name. You can even bring up a list of all coupons by searching “template\_”.

Installing this widget is optional, but we think you’ll find it to be such a handy tool that once you use it, you’ll never want to be without it!

1. Navigate to the Configuration tab and locate the Dashboard Configuration group:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/config_tab_dash.png&w=270&h=54&zc=1&q=100 "Configuration Tab - Dashboard Configuration Group")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/config_tab_dash.png "Configuration Tab - Dashboard Configuration Group")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click on it to display its configuration panel:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/config_dash.png&w=175&h=176&zc=1&q=100 "Dashboard Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/config_dash.png "Dashboard Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. Click on the second “Edit” button towards the bottom of the configuration panel to bring up the Dashboard Modules list:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/dashboard_mods.png&w=270&h=113&zc=1&q=100 "Dashboard Modules List")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/dashboard_mods.png "Dashboard Modules List")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

7. Click on the Coupon Search module and then click the “Install” button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/coupon_search_install.png&w=175&h=69&zc=1&q=100 "Install the Coupon Search Module")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/coupon_search_install.png "Install the Coupon Search Module")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

9. Click the “Edit” button to bring up the Coupon Search configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/coupon_search_config.png&w=175&h=122&zc=1&q=100 "Configure the Coupon Search Module")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/coupon_search_config.png "Configure the Coupon Search Module")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

11. As you can see from the image above, the module is already set to “True”, meaning it is active. If you want to move the module to a different spot on your MailBeez Interface Dashboard, you may do so by changing the “Sort Order” configuration setting.
12. When you’ve completed your configurations, click the “Update” button
13. The Coupon Search Dashboard Widget is now visible on your MailBeez Dashboard:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/coupon_search_widget.png&w=270&h=94&zc=1&q=100 "The Coupon Search Dashboard Widget")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/coupon_search_widget.png "The Coupon Search Dashboard Widget")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Configuration of the Nopurchase Advanced module is now complete!

 

## Create & Assign Coupon Templates

Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return to the module to assign a coupon template to each email cycle using the drop down box in each email cycle’s configuration panel (see the section of the tutorial on configuring email cycles).

Once you’ve done that, it’s time to test & run some simulations.

 

## Test & Run the Nopurchase Emails

Now that you’ve completed configuration of your module, it’s time to test!

1. Navigate back to the Nopurchase Advanced module in the MailBeez module tab.
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
