---
# http://learn.getgrav.org/content/headers
title: MailBeez ReferralHoney
slug: mailbeez-referralhoney-configuration-tutorial
# menu: MailBeez ReferralHoney
date: 30-08-2012
published: true
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

Übersetzung folgt

The screenshots used in this tutorial were made using Zen Cart. If you use a different e-commerce platform, your admin interface and MailBeez interface may appear slightly different, however the concepts and configuration instructions are the same across all platforms.

## About This Module

ReferralHoney emails a personalized coupon code link to each customer after they have placed an order in your store, which they can then share with friends, family or co-workers, with the knowledge that if one of their contacts places an order with the code, they will automatically receive a store reward.

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the ReferralHoney module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/install.png&w=175&h=78&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_config.png&w=175&h=470&zc=1&q=100 "ReferralHoney Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_config.png "ReferralHoney Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring ReferralHoney

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/general_settings.png&w=175&h=793&zc=1&q=100 "ReferralHoney General Settings")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/general_settings.png "ReferralHoney General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Target Order Status, Target Days Since Last Purchase, Target Days to to Look Back & Last Invitation Delay**  
 These 4 settings work together to identify eligible customers & create a window of time in which MailBeez will look for them when the ReferralHoney module is run.

**Target Customer Order Status & Target Customer’s Friend’s Order Status**  
 This setting lets you define which order status the module should target as eligible to trigger a Referral Invitation email. By default, it is set to an order status of “Delivered”, “Completed”, or “Dispatched”, depending on your e-commerce platform. Customers and customers’ friends who have an order status that matches this setting and who fall within the time frame parameters defined in the next three settings will receive a Referral Invitation email when this module is run.

**Target Days Since Last Purchase**  
 This setting tells MailBeez to target orders “X” number of days after they reach the required order status as defined by the “Target Order Status” setting. By default it is set to “2”, meaning that orders which have reached the required order status 2 or more days ago are eligible to receive a Referral Invitation email when the ReferralHoney module is run.

**Target Days to Look Back**  
 This setting lets you define how far back in time MailBeez should look for customers and customer’s friends who meet the “Order Status” and “Days Since Last Purchase” criteria. By default, it is set to 10 and must always be a higher number than the “Days Since Last Purchase” setting.

**Last Invitation Delay**  
 This setting lets you control the number of days MailBeez must wait between sending two separate invitations to the same customer. It filters out customers who have orders which meet the “Days Since Last Purchase” & “Days to Look Back” criteria, but have already received a Referral Invitation email within the last “X” number of days. By default, it is set to 90 days.

Without this setting, the module would generate a Referral Invitation email to every customer for every order once it meets the “Order Status” and “Days to Look Back” criteria.

As you can imagine, this would get rather annoying to customers who place orders frequently, so you want to keep the number fairly high – somewhere between 60 and 90. If you don’t have customers who do frequent repeat business, lowering this number slightly would be reasonable. 30 days is a good example.

The default settings of:

- Order Status = Delivered
- Days Since Last Purchase = 2
- Days to Look Back = 10
- Last Invitation Delay = 90

all work together to tell MailBeez “Search my database for the past 10 days. Find all orders which have reached an order status of “Delivered” 2 or more days ago. Of those you find, filter out any orders from customers who received a Referral Invitation in the last 90 days. Send the remaining customers a Referral Invitation email.”

**Share Coupon – Days Coupon is Valid**  
 The Share Coupon is the coupon you send to your customers so they can share it with others. This setting allows you define the number of days the Share Coupon will be valid. After these number of days pass, the coupon will expire. By default, it is set to 15 days, but you may change it if you wish.

**Reward Coupon – Days Coupon is Valid**  
 The Reward Coupon is the coupon you send to your customers to reward them after their friends make a purchase with the Share Coupon. This setting allows you define the number of days the Reward Coupon will be valid. After these number of days pass, the coupon will expire. By default, it is set to 66 days, but you may change it if you wish.

**Consider adding the [Coupon Expiry Reminder](/documentation/mailbeez/coupon_expire/) module to your MailBeez installation to increase the conversion rate of coupon emails and thereby generate more sales! Powerful!**

**Length of Coupon Code**  
 This setting allows you to define the length of the coupon code that MailBeez will generate. By default it is set to 10 characters. You may change it if you wish, keeping in mind that the longer the code, the more character combinations are possible. If you make this code too short, you could limit the number of available character combinations, thereby limiting the number of unique coupon codes that MailBeez can generate.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Layout**  
 This setting allows you to choose which layout style template set you want to assign & use for this module.

Since ReferralHoney does not include additional templates, the only option displayed here is “Default” until such a time as you create your own custom templates. For help creating your own custom templates, check out our [Customizing Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

Once you’ve completed your configurations, click the “Update” button.

### Configure the Referral Invitation Email Cycle

The Referral Invitation email is sent to anyone who places an order once that order meets the “Order Status”, “Days Since Last Purchase”, “Days to Look Back”, & “Last Invitation Delay” criteria.

1. Click on the Referral Invitation email cycle option beneath the module name on the MailBeez Modules tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/email_cycle1.png&w=270&h=45&zc=1&q=100 "Referral Invitation Email Cycle")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/email_cycle1.png "Referral Invitation Email Cycle")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/1st_email_config.png&w=175&h=341&zc=1&q=100 "Referral Invitation Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/1st_email_config.png "Referral Invitation Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Target Days Since Last Purchase**  
 This setting is identical to its counterpart in the module’s general configuration settings and is placed here for convenience. Changing the setting in this panel will automatically update it the module’s general configurations panel. The converse is also true; changing the setting in the module’s general configurations panel will update the setting here in this panel.

Whatever you enter here will display next to the Referral Invitation email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your setting is. Handy!

**Coupon Template – Share With Friends Coupon**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

**Share Coupon – Days Coupon is Valid**  
 This setting is identical to its counterpart in the module’s general configuration settings and is placed here for convenience. Changing the setting in this panel will automatically update it the module’s general configurations panel. The converse is also true; changing the setting in the module’s general configurations panel will update the setting here in this panel.

**Target Customer’s Order Status**  
 This setting is identical to its counterpart in the module’s general configuration settings and is placed here for convenience. Changing the setting in this panel will automatically update it the module’s general configurations panel. The converse is also true; changing the setting in the module’s general configurations panel will update the setting here in this panel.

Once you’ve completed your configurations, click the “Update” button.

### Configure the Friend Made a Purchase Email Cycle

This email is sent to customers each time one of their friends uses the Share Coupon to make a purchase in your store. It is a courtesy email designed to keep the customer up to date so they can anticipate their Referral Bonus or even be motivated to continue sharing the Share Coupon.

1. Click on the Friend Made a Purchase email cycle option beneath the module name on the MailBeez Modules tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/email_cycle2.png&w=270&h=52&zc=1&q=100 "Friend Made a Purchase Email Cycle")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/email_cycle2.png "Friend Made a Purchase Email Cycle")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/2nd_email_config.png&w=175&h=160&zc=1&q=100 "Friend Made a Purchase Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/2nd_email_config.png "Friend Made a Purchase Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Target Customer’s Friend’s Order Status**  
 This setting is identical to its counterpart in the module’s general configuration settings and is placed here for convenience. Changing the setting in this panel will automatically update it the module’s general configurations panel. The converse is also true; changing the setting in the module’s general configurations panel will update the setting here in this panel.

Once you’ve completed your configurations, click the “Update” button.

### Configure the Referral Bonus Email Cycle

The Referral Bonus email is sent to customers “X” number of days after the Share Coupon expires. It provides your customers with the total number of orders resulting from their Share Coupon as well as the resulting Reward Coupon. If the customer’s Share Coupon was never used, the email is sent explaining that the coupon expired without having been used and assures them that they will get another opportunity to earn a Reward Coupon next time they shop with you.

1. Click on the Referral Bonus email cycle option beneath the module name on the MailBeez Modules tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/email_cycle3.png&w=270&h=60&zc=1&q=100 "Referral Bonus Email Cycle")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/email_cycle3.png "Referral Bonus Email Cycle")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/3rd_email_config.png&w=175&h=537&zc=1&q=100 "Referral Bonus Email Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/3rd_email_config.png "Referral Bonus Email Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Target Days Since Coupon Expiry**  
 This setting lets you tell MailBeez how many days to wait after the Share Coupon expires before sending out the Referral Bonus email. By default, it is set to 2.

**Number of Orders for Level 1**  
 This setting lets you define how many recognized orders a Share Coupon must generate for the customer to receive a Level 1 Reward Coupon. A “recognized” order is any order meeting the “Target Customer’s Friend’s Order Status” criteria. By default, it is set to 1.

**Coupon Template – Reward Level 1**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

**Number of Orders for Level 2**  
 This setting lets you define how many recognized orders a Share Coupon must generate for the customer to receive a Level 2 Reward Coupon. A “recognized” order is any order meeting the “Target Customer’s Friend’s Order Status” criteria. By default, it is set to 3.

**Coupon Template – Reward Level 2**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

**Number of Orders for Level 3**  
 This setting lets you define how many recognized orders a Share Coupon must generate for the customer to receive a Level 3 Reward Coupon. A “recognized” order is any order meeting the “Target Customer’s Friend’s Order Status” criteria. By default, it is set to 10.

**Coupon Template – Reward Level 3**  
 This setting allows you to assign a coupon template to this email cycle option using the dropdown box which will be visible once you create at least one coupon template. Until then, you will only see a link that takes you to your store’s coupon administration area . Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return here to assign a template to this email cycle.

**Reward Coupon – Days Coupon is Valid**  
 This setting is identical to its counterpart in the module’s general configuration settings and is placed here for convenience. Changing the setting in this panel will automatically update it the module’s general configurations panel. The converse is also true; changing the setting in the module’s general configurations panel will update the setting here in this panel.

Once you’ve completed your configurations, click the “Update” button.

 

## The Coupon Engine

The ReferralHoney module adds a new configuration group to your MailBeez installation: Coupon Engine configuration. This is a common configuration group shared by multiple premium email modules. If you have already configured this group after installing another module, you may skip these steps.

Otherwise:

1. Navigate to the Configuration tab of the MailBeez interface:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/config_tab3.png&w=270&h=174&zc=1&q=100 "MailBeez Configuration Tab")](http://mailbeez.com/images/doc/common_images/config_tab3.png "MailBeez Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Locate and click on ‘Coupon Engine’ to bring up the Coupon Engine configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/common_images/coupon_engine_config.png&w=175&h=154&zc=1&q=100 "Coupon Engine Configuration Panel")](http://mailbeez.com/images/doc/common_images/coupon_engine_config.png "Coupon Engine Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. As you can see from the image above, there are no actual settings here to configure, but you need to be aware of this configuration option because it allows you to delete all simulation coupons. When you run simulations, MailBeez will create simulated coupon codes which are unnecessary once simulations are complete. Once you’ve completed all your simulated runs of this module, return here and click on the “Delete” button to delete the simulation coupons.

 

## Install ReferralHoney Statistics Report

The ReferralHoney module adds the framework for a new statistics report to your MailBeez installation: the ReferralHoney Statistics Report . This report will gather and display all of your ReferralHoney statistics in one place! Although the report display is currently under development, you can still navigate through this area to get an idea of what to expect.

Or, feel free to skip these steps until an updated version of the module has been released.

1. Navigate to the Reports tab of your MailBeez interface and locate the ReferralHoney Statistics module:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/reports_tab.png&w=270&h=52&zc=1&q=100 "Reports Tab - ReferralHoney Statistics")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/reports_tab.png "Reports Tab - ReferralHoney Statistics")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click on “ReferralHoney Statistics” and then click on its “Install” button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_statistics_install.png&w=175&h=71&zc=1&q=100 "Install Configuration Settings Into Your Database")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_statistics_install.png "Install Configuration Settings Into Your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. Click the “Edit” button to bring up its configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_statistics_config.png&w=175&h=133&zc=1&q=100 "Configure the ReferralHoney Statistics Module")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_statistics_config.png "Configure the ReferralHoney Statistics Module")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

7. As you can see from the image above, there’s not much to do here because the module is already set to “True”, meaning it is active. If you want to move the module to a different location on the Report List, you may do so by changing the “Sort Order” configuration setting.
8. When you’ve completed your configurations, click the “Update” button
9. To access the ReferralHoney Statistics Report, click on the “Open Analytics” button on the configuration panel:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_statistics_open.png&w=175&h=173&zc=1&q=100 "Access the ReferralHoney Statistics Report")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_statistics_open.png "Access the ReferralHoney Statistics Report")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

11. Once this feature completes development, you’ll be able to see all of your ReferralHoney Analytics Statistics all in one place. Until then, you will see this:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_statistics_report.png&w=270&h=74&zc=1&q=100 "New Install ReferralHoney Statistics Report")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_statistics_report.png "New Install ReferralHoney Statistics Report")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


 

## The ReferralHoney Dashboard Widget

The ReferralHoney module adds a new dashboard widget to your MailBeez installation: the ReferralHoney Analytics Dashboard Widget.

1. Navigate to the Configuration tab and locate the Dashboard Configuration group:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/config_tab_dash.png&w=270&h=54&zc=1&q=100 "Configuration Tab - Dashboard Configuration Group")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/config_tab_dash.png "Configuration Tab - Dashboard Configuration Group")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click on it to display its configuration panel:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/config_dash.png&w=175&h=176&zc=1&q=100 "Dashboard Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/nopurchase_advance/config_dash.png "Dashboard Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. Click on the second “Edit” button towards the bottom of the configuration panel to bring up the Dashboard Modules list:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/dashboard_mods.png&w=270&h=113&zc=1&q=100 "Dashboard Modules List")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/dashboard_mods.png "Dashboard Modules List")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

7. Click on the ReferralHoney Analytics module to bring up the ReferralHoney Analytics configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/widget_config.png&w=175&h=148&zc=1&q=100 "Configure the Referral Honey Widget")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/widget_config.png "Configure the Referral Honey Widget")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

9. As you can see from the image above, the module is already set to “True”, meaning it is active. If you want to move the module to a different spot on your MailBeez Interface Dashboard, you may do so by changing the “Sort Order” configuration setting.
10. To change the number of days worth of ReferralHoney Analytics data displayed on the widget graphs change the “Days to Look Back” configuration setting. By default, it is set to 30 and will display a month’s worth of Analytics data in the graphs on the widget.
11. When you’ve completed your configurations, click the “Update” button
12. The ReferralHoney Analytics Dashboard Widget is now visible on your MailBeez Dashboard:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_widget.png&w=270&h=95&zc=1&q=100 "The ReferralHoney Analytics Dashboard Widget")](http://www.mailbeez.com/images/doc/mailbeez/coupon_referral_honey/referralhoney_widget.png "The ReferralHoney Analytics Dashboard Widget")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Configuration of the ReferralHoney module is now complete!

 

## Create & Assign Coupon Templates

Once you’ve finished configuring the module, create your coupon templates using our [**Coupon Template Tutorial**](/documentation/tutorials/coupon-template-tutorial/) as a guide, and then return to the module to assign a coupon template to each email cycle using the drop down box in each email cycle’s configuration panel (see the section of the tutorial on configuring email cycles).

Once you’ve done that, it’s time to test & run some simulations.

 

## Customize Your Share Page

The Share Link included in the ‘Referral Invitation’ & ‘Friend Made a Purchase’ emails will take those who click on it to a ‘Share Page’ which contains a link to your store and the coupon code friends & family need to enter at checkout in order to receive their discount.

To customize the Share Page, simply edit the template which controls it using HTML:

mailhive/mailbeez/coupon\_referral\_honey/templates/sharepage.tpl.html

 

## Test & Run the ReferralHoney Emails

Now that you’ve completed configuration of your module, it’s time to test!

1. Navigate back to the ReferralHoney module in the MailBeez module tab.
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
