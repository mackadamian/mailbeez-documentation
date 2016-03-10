---
# http://learn.getgrav.org/content/headers
title: Review Reminder Advanced
slug: ID-5739
# menu: Review Reminder Advanced
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

The screenshots used in this tutorial were made using Zen Cart. If you use a different e-commerce platform, your admin interface and MailBeez interface may appear slightly different, however the concepts and configuration instructions are the same across all platforms.

## About This Module

Review Reminder Advanced allows you to contact customers after a purchase in a non-invasive and newsletter status intelligent manner to invite them to leave product reviews in your store. When customers leave product reviews, SEO is improved due to the increased page content provided by customer reviews, and of course future customers are more encouraged to buy!

Review Reminder Advanced makes it so easy for your customers because it includes a seamless ‘auto login’ feature, which automatically signs your customers into your site on click through from the review email, allowing them to start writing straight away. For additional security, the auto login feature is only valid for writing reviews, so other pages of the site, like the “my account” area for example, still require a manual login with their user credentials.

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Review Reminder Advanced module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/install.png&w=175&h=86&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/config_panel.png&w=175&h=443&zc=1&q=100 "Review Reminder Advanced Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/config_panel.png "Review Reminder Advanced Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring Review Reminder Advanced

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/general_settings.png&w=175&h=642&zc=1&q=100 "Review Reminder Advanced General Settings")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/general_settings.png "Review Reminder Advanced General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Order Status Trigger, Minimum Age of Order & Number of Days to to Look Back**  
 These 3 settings work together to identify eligible customers & create a window of time in which MailBeez will look for them when the Review Reminder Advanced module is run.

**Order Status Trigger**  
 This setting lets you define the order status an order must have to trigger a Review Reminder email to be sent. By default, it is set to an order status of “Delivered”, “Completed”, or “Dispatched”, depending on your e-commerce platform. Customers who have an order status that matches this setting and who fall within the time frame parameters defined in the next two settings will receive a Review Reminder email when this module is run.

**Minimum Age of Order**  
 This setting tells MailBeez to target orders “X” number of days after they reach the required order status as defined by the “Order Status Trigger” setting. By default it is set to “10”, meaning that orders which have reached the configured “Order Status” 10 or more days ago are eligible to receive a Review Reminder Email when the Review Reminder Advanced module is run.

**Number of Days to Look Back**  
 This setting lets you define how far back in time MailBeez should look for customers who meet the Order Status and Minimum Age of Order criteria. By default, it is set to 20 and must always be a higher number than the “Minimum Age of Order” setting.

You may want to set this to a higher number for your initial run of the module in order to invite more customers to write a review – but don’t set it too high or you’ll be inappropriately emailing customers with old purchases. 60 is an example of a good setting for an initial run, but don’t forget to lower the number after the initial run. Otherwise MailBeez will be needlessly looking further back than it has to on subsequent runs.

**How it Works & Changing Settings**  
 The default settings of: Order Status = Delivered, Minimum Age of Order = 10, and Days to Look Back = 20 all work together to tell MailBeez “Search my database for the past 20 days and find all orders which have reached an order status of Delivered 10 or more days ago, and send them a Review Reminder email.”

Since “Days to Look Back” is set to 20, and “Minimum Age of Order’ is set to 10, this means MailBeez will find 2 batches of customers who meet the “Minimum Age of Order” criteria (20 divided by 10 = 2).

This is important because if a run of this module fails and a batch of customers are missed, they will get picked up in the next run. So it is a good idea to set “Number of Days to Look Back” to a number which is double that of “Minimum Age of Order”. For example, if you change “Minimum Age of Order” to 5, then you would want to change “Number of Days to Look Back” to 10.

**Workflow – Number of Review Invitations (1-3)**  
 This setting lets you control how many Review Reminder email cycles you want the module to complete for each customer meeting the criteria to receive Review Reminder emails. By default, this setting is set to 2, however you may send as few as 1 or as many as 3.

The number you select here also controls which email cycle options are displayed beneath the module name in the MailBeez Modules tab & are therefore available for configuration, testing, and use. Images of this concept are below.

**For each email cycle, MailBeez will disregard customers who have already received a Review Reminder email from that cycle, ensuring that a customer will not receive the same email from the same cycle more than once. **

**Send 1 Email**  
 Setting this to 1 will result in only the ‘Initial Invitation to Write a Review’ email cycle option being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/email_cycle1.png&w=270&h=38&zc=1&q=100 "Review Reminder Advanced Email Cycle Option 1")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/email_cycle1.png "Review Reminder Advanced Email Cycle Option 1")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive only one email inviting them to write a review. If they fail to write a product review, they will not be reminded again.

**Send 2 Emails**  
 Setting this to 2 will result in the ‘Initial Invitation to Write a Review’ and ‘First Reminder’ email cycle options being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/email_cycle2.png&w=270&h=46&zc=1&q=100 "Review Reminder Advanced Email Cycle Option 2")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/email_cycle2.png "Review Reminder Advanced Email Cycle Option 2")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive the initial invitation email inviting them to write a review. If they fail to write a product review, they will receive a reminder email “X” number of days later, based on your configuration settings. More on this configuration setting later.

If you plan on setting your email cycles to 2, you may wish to include some language in your layout style step 2 email template indicating that this will be the final reminder. Doing so will reassure a customer who doesn’t intend to write a review that you won’t continue to ask them to, and may encourage a customer who does intend to write a review to do so upon receipt of the email

**Send 3 Emails**  
 Setting this to 3 will result in the ‘Initial Invitation to Write a Review’, ‘First Reminder’, and ‘Second Reminder’ email cycle options being displayed in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/email_cycle3.png&w=270&h=52&zc=1&q=100 "Review Reminder Advanced Email Cycle Option 3")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/email_cycle3.png "Review Reminder Advanced Email Cycle Option 3")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The customer will receive the initial invitation email inviting them to write a review. If they fail to write a product review, they will receive a reminder email “X” number of days later, based on your configuration settings. If the customer again fails to write a product review, a final review reminder email will be sent “X” number of days later, based on your configuration settings. More on this configuration setting later.

Be careful with this setting. If you decide to use the Second Reminder email option, remember that you will be sending them 3 emails about the same subject. You will want to be sure to use some careful & creative wording in your layout style step 3 email templates to avoid a situation where your customers feel nagged or harassed.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Enable Autologin**  
 This setting enables and disables the autologin feature of this module. It is set to “True” by default, meaning that autologin is enabled. We recommend that you leave this setting enabled because it allows customers to write reviews without having to log in to their account, and since the autologin is only valid for review writing, no other area of the customer account can be accessed, ensuring their account data remains secure.

**In order for this feature to function, you needed to add two small blocks of code to one of your store’s files. See the installation instructions included in the download package for details.**

**Layout**  
 This setting allows you to choose which layout style template set you want to assign & use for this module.

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

**Random Products for Testing**  
 MailBeez Premium modules display actual product lists in your test emails, enabling you to see what the product list looks like in the various layout style templates. Additionally, if you utilize the List Engine configuration settings to change the layout and appearance of your product lists in your email templates, this feature will allow you to preview those changes in test emails prior to you sending the emails to your customers.

The configuration setting is already pre-populated with random product id’s from your store, but you may change them if you wish to use specific products in your testing.

Once you’ve completed your configurations, click the “Update” button.

### Configure the Initial Invitation Email Cycle

1. Click on the Initial Invitation email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/initial_invite_config.png&w=175&h=103&zc=1&q=100 "Initial Invitation Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/initial_invite_config.png "Initial Invitation Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Minimum Age of Order**  
 This setting is identical to its counterpart in the module’s general configuration settings and is placed here for convenience. Changing the setting in this panel will automatically update it the module’s general configurations panel. The converse is also true; changing the setting in the module’s general configurations panel will update the setting here in this panel.

Whatever you enter here will display next to the Initial Invitation email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your setting is. Handy!

### Configure the First Reminder Email Cycle

1. Click on the First Reminder email cycle option beneath the module name on the MailBeez Modules tab
2. Click the “Edit” button to bring up the configuration settings panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/first_reminder_config.png&w=175&h=96&zc=1&q=100 "First Reminder Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/first_reminder_config.png "First Reminder Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Number of Days Delay After Initial Invitation**  
 This setting is identical to its counterpart in the module’s general configuration settings and is placed here for convenience. Changing the setting in this panel will automatically update it the module’s general configurations panel. The converse is also true; changing the setting in the module’s general configurations panel will update the setting here in this panel.

Whatever you enter here will display next to the Initial Invitation email cycle option on the MailBeez Modules tab, so you can always see, at a glance, what your setting is. Handy!

 

## Configure List Engine & Social Sharing Settings

The Review Reminder Advanced module adds two new configuration groups to your MailBeez installation: List Engine configuration and Social Sharing configuration.

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

The Review Reminder Advanced module adds two new filters to your MailBeez installation: the Check Review filter and the Layout Optimizer filter.

1. Navigate to filter & helper tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/filter_tab2.png&w=270&h=68&zc=1&q=100 "MailBeez Filter & Helper Tab")](http://www.mailbeez.com/images/doc/common_images/filter_tab2.png "MailBeez Filter & Helper Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click on the Check Review filter and then click its ‘Install’ button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/review_check_filter_install.png&w=175&h=84&zc=1&q=100 "Install Review Check Filter")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/review_check_filter_install.png "Install Review Check Filter")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. Click on the “Edit” button to bring up the filter’s configuration settings:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/review_advanced/review_check_filter_config.png&w=175&h=80&zc=1&q=100 "Review Check Filter Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/review_advanced/review_check_filter_config.png "Review Check Filter Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

As you can see from the image above, there is only one configuration setting here – activate or deactivate the filter. It is set to “True” by default, meaning the filter is active.

However, the Check Review filter is only necessary if you were running the Review Reminder Simple module prior to installing the advanced module. It’s function is to prevent the advanced module from resending to clients already contacted by simple module. It also checks to see if customers have blocked the simple module, and if so, blocks them from receiving the advanced module mailings.

9. If you were not using the Review Reminder Simple module, change this setting to “False” to disable it.
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

 

## Test & Run the Invitation & Reminder Emails

Now that you’ve completed configuration of your module, it’s time to test!

1. Navigate back to the Review Reminder Advanced module in the MailBeez module tab.
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



## Additional Review Modules

- Reward customers who write reviews with a coupon for their next purchase by installing the [MailBeez Review Reward Coupon module!](/documentation/mailbeez/coupon_review/)
- Have you seen the [MailBeez Share Review on Facebook module](/documentation/mailbeez/review_facebook/)? This **free** module will send an email to customers who have written a review inviting them to share their review on Facebook. The simple one-click operation makes sharing a breeze for your customers!

## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.

## Template Manager

Mailbeez has developed a handy module that easily allows you to both edit and view your text changes right from the MailBeez interface within your store’s admin. Fully functional with all official MailBeez Modules (free, premium, and custom built), the MailBeez Template Manager makes editing a template a breeze, so much so that you may wonder how you ever lived without it! **[ Learn more!](/documentation/configbeez/config_tmplmngr/)**
