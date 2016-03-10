---
# http://learn.getgrav.org/content/headers
title: Winback Advanced
slug: ID-5741
# menu: Winback Advanced
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

In order to prevent formerly good customers from falling through the cracks of your marketing strategy, Mailbeez has developed a deceptively powerful, fully automated module called Winback Advanced, which gives you the tools you to email old customers who haven’t placed an order for a pre-determined time span (set in the admin area), both reminding them of your presence, and enticing them back with personalised offers & coupons.

With Winback Advanced, not only can you send a personalized one-off coupon to formerly long lost customers, but as part of its multi-step architecture, if the customer still isn’t returning, Winback can raise the stakes over a series of emails with pre-configured time delays, all embedded with offer coupons that can be set to increase in value in line with the multi-step process, until the customer simply cannot resist the deal you are offering.

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Winback Advanced module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/install.png&w=175&h=78&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/winback_config.png&w=175&h=460&zc=1&q=100 "Winback Advanced Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/winback_config.png "Winback Advanced Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring Winback Advanced

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/general_settings.png&w=175&h=703&zc=1&q=100 "Winback Advanced General Settings")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/general_settings.png "Winback Advanced General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Target Order Status, Target Days Since Last Purchase & Target Days to to Look Back**  
 These 3 settings work together to identify eligible customers & create a window of time in which MailBeez will look for them when the Winback Advanced module is run.

**Target Order Status**  
 This setting lets you define the order status the module should target as eligible to receive a Winback email. By default, it is set to an order status of “Delivered”, “Completed”, or “Dispatched”, depending on your e-commerce platform. Customers who have an order status that matches this setting and who fall within the time frame parameters defined in the next two settings will receive a Winback email when this module is run.

**Target Days Since Last Purchase**  
 This setting tells MailBeez to target orders “X” number of days after they reach the required order status as defined by the “Target Order Status” setting. By default it is set to “90”, meaning that orders which have reached the required order status 90 or more days ago are eligible to receive a Winback email when the Winback Advanced module is run.

**Target Days to Look Back**  
 This setting lets you define how far back in time MailBeez should look for customers who meet the “Order Status” and “Days Since Last Purchase” criteria. By default, it is set to 120 and must always be a higher number than the “Days Since Last Purchase” setting.

**How it Works & Changing Settings**  
 The default settings of: Order Status = Delivered, Days Since Last Purchase = 90, and Days to Look Back = 120 all work together to tell MailBeez “Search my database for the past 120 days and find all orders which have reached an order status of Delivered 90 or more days ago, and send them a Winback email.”

If you set “Days to Look Back” to 180, and leave “Days Since Last Purchase” set to 90, MailBeez will find 2 batches of customers who meet the “Days Since Last Purchase” criteria (180 divided by 90 = 2).

This is important because if a run of this module fails and a batch of customers are missed, they will get picked up in the next run. So it is a good idea to set “Target Days to Look Back” to a number which is double that of “Target Days Since Last Purchase”. For example, if you change “Days Since Last Purchase” to 60, then you would want to set “Days to Look Back” to 120.

**Workflow – Number of Winback Emails (1-4+)**  
 This setting lets you control how many Winback email cycles you want the module to complete for each customer meeting the criteria to receive Winback emails. By default, this setting is set to Loop but you may decrease it if you wish.

The number you select here also controls which email cycle options are displayed beneath the module name in the MailBeez Modules tab & are therefore available for configuration, testing, and use. Images of this concept are below.

**For each email cycle, MailBeez will disregard customers who have already received a Winback email from that cycle, ensuring that a customer will not receive the same email from the same cycle more than once. **

**Send 1 Email**  
 Setting this to 1 will result in only the ‘First Winback’ email cycle option being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/email_cycle1.png&w=270&h=37&zc=1&q=100 "Winback Advanced Email Cycle Option 1")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/email_cycle1.png "Winback Advanced Email Cycle Option 1")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive only one email enticing them back to your store. If they fail to use the enclosed link to return to the store and make a purchase, they will not be emailed again.

**Send 2 Emails**  
 Setting this to 2 will result in the ‘First Winback’ and ‘Second Winback’ email cycle options being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/email_cycle2.png&w=270&h=45&zc=1&q=100 "Winback Advanced Email Cycle Option 2")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/email_cycle2.png "Winback Advanced Email Cycle Option 2")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive the First Winback email enticing them back to your store. If they fail to use the enclosed link to return to the store and make a purchase, they will receive the Second Winback email “X” number of days later, based on your configuration settings. More on this configuration setting later.

**Send 3 Emails**  
 Setting this to 3 will result in the ‘First Winback’, ‘Second Winback’, and ‘Third Winback’ email cycle options being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/email_cycle3.png&w=270&h=61&zc=1&q=100 "Winback Advanced Email Cycle Option 3")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/email_cycle3.png "Winback Advanced Email Cycle Option 3")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive the First Winback email enticing them back to your store. If they fail to use the enclosed link to return to the store and make a purchase, they will receive the Second Winback email “X” number of days later, based on your configuration settings. if the customer again fails to use the enclosed link to return to the store and make a purchase, the Third Winback email will be sent “X” number of days later, based on your configuration settings. More on this configuration setting later.

**Send Loop Emails**  
 Setting this to Loop will result in the ‘First Winback’, ‘Second Winback’, ‘Third Winback’, and ‘Winback Loop’ email cycle options being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/email_cycle4.png&w=270&h=60&zc=1&q=100 "Winback Advanced Email Cycle Option Loop")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/email_cycle4.png "Winback Advanced Email Cycle Option Loop")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive the First Winback email enticing them back to your store. If they fail to use the enclosed link to return to the store and make a purchase, they will receive the Second Winback email “X” number of days later, based on your configuration settings. if the customer again fails to use the enclosed link to return to the store and make a purchase, the Third Winback email will be sent “X” number of days later, based on your configuration settings.

If the customer still fails to use the enclosed link to return to the store and make a purchase, they will begin to receive Winback emails in an ongoing loop as often as you configure the loop to continue. More on this configuration setting later.

Be careful with this setting. If you decide to use the loop option, you’ll want to avoid being flagged by your old customers as a spammer – or worse – reported by your customers to potential customers via social media.

One good way to avoid this is to create a variety of templates and offerings for the loop iteration and change them out between runs of the module. This ensures that customers are always receiving fresh content. To them, it looks like a newsletter. Sending the same content and same offer over and over again just looks like spam.

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

**Random Products for Testing**  
 MailBeez Premium modules display actual product lists in your test emails, enabling you to see what the product list looks like in the various layout style templates. Additionally, if you utilize the List Engine configuration settings to change the layout and appearance of your product lists in your email templates, this feature will allow you to preview those changes in test emails prior to you sending the emails to your customers.

The configuration setting is already pre-populated with random product id’s from your store, but you may change them if you wish to use specific products in your testing.

Once you’ve completed your configurations, click the “Update” button.

### Configure the First Winback Email Cycle

1. Click on the First Winback email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/1st_email_config.png&w=175&h=176&zc=1&q=100 "First Winback Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/1st_email_config.png "First Winback Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Target Days Since Last Purchase**  
 This setting is identical to its counterpart in the module’s general configuration settings and is placed here for convenience. Changing the setting in this panel will automatically update it the module’s general configurations panel. The converse is also true; changing the setting in the module’s general configurations panel will update the setting here in this panel.

Whatever you enter here will display next to the First Winback email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your setting is. Handy!

**Coupon Template – First Winback Email**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

### Configure the Second Winback Email Cycle

1. Click on the Second Winback email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/2nd_email_config.png&w=175&h=177&zc=1&q=100 "Second Winback Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/2nd_email_config.png "Second Winback Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Second Winback Email Delay**  
 This setting allows you to tell MailBeez how many days to wait after sending out the First Winback email before sending out the Second Winback email. By default, it it set to 1, but you should probably increase it. Since each email cycle will ideally contain better and better coupon offers, sending out Winback emails too close together can train your customers to wait for the best offer and possibly cheapen your business reputation.

Whatever you enter here will display next to the Second Winback email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your setting is. Handy!

**Coupon Template – Second Winback Email**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

### Configure the Third Winback Email Cycle

1. Click on the Third Winback email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/3rd_email_config.png&w=175&h=176&zc=1&q=100 "Third Winback Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/3rd_email_config.png "Third Winback Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Third Winback Email Delay**  
 This setting allows you to tell MailBeez how many days to wait after sending out the Second Winback email before sending out the Third Winback email. By default, it it set to 1, but you should probably increase it for the reasons stated above.

Whatever you enter here will display next to the Third Winback email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your setting is. Handy!

**Coupon Template – Third Winback Email**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

### Configure the Loop Winback Email Cycle

1. Click on the Winback Email Loop email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/4th_email_config.png&w=175&h=216&zc=1&q=100 "Loop Winback Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/4th_email_config.png "Loop Winback Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Winback Email Loop Delay**  
 This setting allows you to tell MailBeez how many days to wait after sending out the Third Winback email before starting the Winback Email Loop. By default, it it set to 1, but you should probably increase it for the reasons stated above.

**Winback Loop Period**  
 This setting allows you to tell MailBeez how often, in days, to repeat the Winback email loop. By default, it is set to 1, but you should probably increase it for the reasons stated above.

Whatever you enter for these two settings will display next to the Winback Email Loop email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your settings are. Handy!

**Coupon Template – Loop**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

 

## Coupon Engine, List Engine & Social Sharing

The Winback Advanced module adds three new configuration groups to your MailBeez installation: Coupon Engine configuration, List Engine configuration, and Social Sharing configuration.

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

 

## Install & Configure Additional Filters

The Winback Advanced module adds two new filters to your MailBeez installation: the Check Winback filter and the Layout Optimizer filter.

1. Navigate to filter & helper tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/filter_tab2.png&w=270&h=68&zc=1&q=100 "MailBeez Filter & Helper Tab")](http://www.mailbeez.com/images/doc/common_images/filter_tab2.png "MailBeez Filter & Helper Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click on the Check Winback filter and then click its ‘Install’ button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/winback_check_filter_install.png&w=175&h=84&zc=1&q=100 "Install Winback Check Filter")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/winback_check_filter_install.png "Install Winback Check Filter")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. Click on the “Edit” button to bring up the filter’s configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/winback_check_filter_config.png&w=175&h=80&zc=1&q=100 "Winback Check Filter Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/winback_advanced/winback_check_filter_config.png "Winback Check Filter Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

As you can see from the image above, there is only one configuration setting here – activate or deactivate the filter. It is set to “True” by default, meaning the filter is active.

However, the Check Winback filter is only necessary if you were running the Winback Simple module prior to installing the advanced module. It’s function is to prevent the advanced module from resending to clients already contacted by simple module. It also checks to see if customers have blocked the simple module, and if so, blocks them from receiving the advanced module mailings.

9. If you were not using the Winback Simple module, change this setting to “False” to disable it.
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

Configuration of the module is now complete!

 

## Create & Assign Coupon Templates

Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return to the module to assign a coupon template to each email cycle using the drop down box in each email cycle’s configuration panel (see the section of the tutorial on configuring email cycles).

Once you’ve done that, it’s time to test & run some simulations.

 

## Test & Run the Winback Emails

Now that you’ve completed configuration of your module, it’s time to test!

1. Navigate back to the Winback Advanced module in the MailBeez module tab.
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
