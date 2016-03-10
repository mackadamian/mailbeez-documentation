---
# http://learn.getgrav.org/content/headers
title: MailBeez Feedback
slug: ID-4423
# menu: MailBeez Feedback
date: 11-07-2012
published: false
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

This MailBeez Module sends a monthly statistic email to MailBeez about which modules and e-commerce platforms are most used for the purpose of helping us improve MailBeez.  
  

## What Statistics Are Included in the Email?

- Installed modules – This statistic tells us which modules have been installed.
- Total number of emails sent – This statistic tells us how much the modules are being used. Taken together with the installed modules statistic, we are able to determine the popularity of various modules, which in turns helps us determine if and when it’s appropriate to design and add more features to any given module.
- Your personal greeting – A short personal message that you create in the configuration panel which is included in the feedback email.
- e-commerce platform – This statistic tells us which e-commerce platform you’re using. This helps us to ensure MailBeez/e-commerce compatibility for all of our customers.

**No personal or professional information is collected about you, your store, or your customers.** The MailBeez Feedback Mailer module is strictly for statistical analysis and product improvement. Like all of the MailBeez modules, it can be activated or deactivated any time you choose.  
  

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png&w=270&h=112&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the MailBeez Feedback module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/mailbeez_feedback/feedback_config1.png&w=175&h=120&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/mailbeez_feedback/feedback_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration settings are now available for you to edit

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/mailbeez_feedback/feedback_config2.png&w=175&h=360&zc=1&q=100 "MailBeez Feedback Configuration Settings")](http://www.mailbeez.com/images/doc/mailbeez/mailbeez_feedback/feedback_config2.png "MailBeez Feedback Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring the MailBeez Feedback Module

There are 5 function buttons and 4 configurable settings. We will go through each of them one at a time.

### General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/mailbeez_feedback/feedback_config3.png&w=175&h=204&zc=1&q=100 "MailBeez Feedback General Settings")](http://www.mailbeez.com/images/doc/mailbeez/mailbeez_feedback/feedback_config3.png "MailBeez Feedback General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “True” by default, meaning the module is on and ready to work. Change this setting to “False” to deactivate the module and disable it from being run.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Your Personal Message**  
 This setting allows you to include a brief personal message in the feedback email that is sent to MailBeez. It is pre-populated with a sample message that you can change or remove.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!  
  

### Test & Run the MailBeez Feedback Module

The 5 function buttons are the controls that allow you to test the module and then manually run it when you’re ready:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/function_buttons.png&w=175&h=184&zc=1&q=100 "Function Buttons")](http://www.mailbeez.com/images/doc/common_images/function_buttons.png "Function Buttons")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Email Templates – “HTML” Button**  
 This button allows you to preview the module templates in a nice popup window in HTML format. This way, you can easily see what the email template looks like and quickly determine which aspects of the template you’ll want to customize for your use.

As you modify your template files, you can come back and use this button to view your changes to ensure that they are appearing as you intend.

When you’re ready to customize your email templates, have a look at our[ Customizing Free Email Templates Tutorial](/documentation/tutorials/customizing-mailbeez-free-email-templates/)

**Email Templates – “TXT” Button**  
 This button allows you to preview the module templates in a nice popup window in text format. Everyone has customers who prefer to receive email in text format. This tool allows you to see what they see, and preview changes you make to the template before they go out to your customers.

**Recipients – “Show” Button**  
 Clicking this button will result in a nice popup window in your admin which is populated with the MailBeez email address to which the information is being sent, along with the actual statistical data that has been gathered so you can be confident about what you’re sending to MailBeez.

**Send Test Email – “Send” Button**  
 This button does just what it says – it lets you send a test email with test data.

**Run this module – “Run” Button**  
 This is the button you use to actually run the module. This button respects your run mode as it is set in your Simulation Configuration, so if you’re in Simulation Mode, clicking this button results in a simulation run. If you are in Production Mode, clicking this button results in a production run.

It even tells you in the text above the button which mode you’re in. This prevents you from accidentally sending emails out to customers when you’re testing.



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.

## Template Manager

Mailbeez has developed a handy module that easily allows you to both edit and view your text changes right from the MailBeez interface within your store’s admin. Fully functional with all official MailBeez Modules (free, premium, and custom built), the MailBeez Template Manager makes editing a template a breeze, so much so that you may wonder how you ever lived without it! **[ Learn more!](/documentation/configbeez/config_tmplmngr/)**
