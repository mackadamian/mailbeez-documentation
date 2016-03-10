---
# http://learn.getgrav.org/content/headers
title: Welcome Email
slug: ID-6184
# menu: Welcome Email
date: 18-09-2012
published: false
publish_date: 18-09-2012
# unpublish_date: 18-09-2012
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

If you’re running Zen Cart v1.5.0+, then you’re aware the development team did away with the built in Welcome email. With this wonderful module from MailBeez, you can bring the Welcome email back to your Zen Cart installation!

If you run one of the other e-commerce platforms, you might be thinking that this module simply doubles up on the email that your shopping cart system already sends when a customer creates an account.

However, with some creative thinking, this secondary ‘welcome’ email can be used for some really interesting ideas, like providing additional store information, or to alert the customer to current special offers.

With the rise on social commerce, this email could even be exclusively tailored to attract visitors to your Facebook or Twitter pages.

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the MailBeez Modules tab:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png&w=270&h=160&zc=1&q=100 "MailBeez Module Tab")](http://www.mailbeez.com/images/doc/common_images/mailbeez_tab2.png "MailBeez Module Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Welcome Email module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/create_account/install.png&w=175&h=70&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/mailbeez/create_account/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/create_account/welcome_config.png&w=175&h=634&zc=1&q=100 "Welcome Email Configuration Panel")](http://www.mailbeez.com/images/doc/mailbeez/create_account/welcome_config.png "Welcome Email Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configure the Welcome Email Module

### Unlock the Module

1. Click on the Certificate “Edit” button
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to be configured.

### Configure General Settings

Click the “Edit” button to access the configurable settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/mailbeez/create_account/general_settings.png&w=175&h=318&zc=1&q=100 "Welcome Email General Settings")](http://www.mailbeez.com/images/doc/mailbeez/create_account/general_settings.png "Welcome Email General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “False” by default, meaning the module is off and will not send emails to customers. Change this setting to “True” to activate the module and enable it to send emails when the module is run.

**Delay After Account Creation & Number of Days to Look Back**  
 These settings work together to create a window of time in which MailBeez will look for opportunities to send the Welcome email by targeting customers who fall within the time frame you define with these settings.

**Delay After Account Creation**  
 This setting lets you define how long you want MailBeez to wait after a new account is created before the Welcome email is sent out. By default, it is set to “0″, meaning that when the module is run, a welcome email will go out to to newly created accounts without delay.

**Number of Days to Look Back**  
 This setting tells MailBeez how far back in time it should look to find customers meeting the “Delay After Account Creation” criteria. By default, it is set to “2″, meaning that when the module is run, it will look for new accounts created within the past two days and send them a Welcome email. As with all MailBeez modules, MailBeez will ignore customers who have already received an email from this module.

Something you want to keep in mind about this module is that the obvious goal is to welcome new customers to your store, therefore, you will want to run it every day if you use the default settings. You can increase the settings if you prefer to run it less often, but the result is that customers will wait longer to be welcomed to your store.

A better strategy is to automate this module to run daily. If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually run this module by clicking the “Run” button in the module as often as you want to run it. The Run MailBeez Automatically module is recommended because it is by far the easier and more reliable of the two options.

**Sender Email**  
 This setting lets you control the email address that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the email address setting that you configured in your store, but you can change it if you prefer.

**Sender Name**  
 This setting lets you control the sender name that is displayed as the sender in your outgoing MailBeez emails. By default, it uses the sender name setting that you configured in your store, but you can change it if you prefer.

**Layout**  
 This setting allows you to choose which layout style template set you want to assign & use for this module.

Since the Welcome Email module does not include additional templates, the only option displayed here is “Default” until such a time as you create your own custom templates. For help creating your own custom templates, check out our [Customizing Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the MailBeez Modules tab.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!

 

## Test & Run the Module

Navigate back to the Welcome Email module in the MailBeez module tab and click on it to display the function buttons on its configuration panel.

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



## Template Manager

Mailbeez has developed a handy module that easily allows you to both edit and view your text changes right from the MailBeez interface within your store’s admin. Fully functional with all official MailBeez Modules (free, premium, and custom built), the MailBeez Template Manager makes editing a template a breeze, so much so that you may wonder how you ever lived without it! **[ Learn more!](/documentation/configbeez/config_tmplmngr/)**
