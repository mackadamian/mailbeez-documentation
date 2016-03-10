---
# http://learn.getgrav.org/content/headers
title: MailBeez Quick Start Configuration
slug: mailbeez-quick-start-configuration-tutorial
# menu: MailBeez Quick Start Configuration
date: 16-07-2012
published: true
publish_date: 16-07-2012
# unpublish_date: 16-07-2012
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

This Quick Start Configuration tutorial will help you get your MailBeez installation configured and ready for testing fast. However, if you’re willing to spend a few more minutes up front, [go to the Comprehensive Configuration tutorial](/documentation/tutorials/mailbeez-comprehensive-configuration-tutorial/) which will need to be completed before you take your store from Simulation to Production Mode and takes approximately 15 – 30 minutes to complete.

The screenshots used in this tutorial were made using Zen Cart. If you use a different e-commerce platform, your admin interface and MailBeez interface may appear slightly different, however the concepts and configuration instructions are the same across all platforms.

## Getting Started

Navigate to your MailBeez Dashboard in your store admin and click on the “Configuration” tab. You will see a number of configuration groups, as shown in the screenshot below:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab.png&w=270&h=134&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In this Quick Start Configuration tutorial, we will focus only on the two configuration groups necessary to get you up and running for testing: MailHive Basic Configuration and Simulation Configuration.

## Basic Configuration

The 9 configurable settings in the Basic Configuration group are mostly self explanatory, but we will go through them one by one:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/configuration/config_mailhive.png&w=175&h=323&zc=1&q=100 "Basic Configuration Settings")](http://mailbeez.com/images/doc/configuration/config_mailhive.png "Basic Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### General Settings

**Let MailBeez Do the Work For You**  
 This setting activates and deactivates MailBeez. It is set to “True” by default, meaning that MailBeez is active and ready to work!

MailBeez defaults to simulation mode upon installation, so it is safe to play around with and test MailBeez without worrying that the emails will be sent to your customers.

There is no need to change this setting unless you want to uninstall or deactivate for MailBeez for some reason. When MailBeez is deactivated (set to “False”), no MailBeez modules will be processed and no emails will be sent, regardless of which mode you are in (simulation or production).

**Show Email While Sending**  
 This setting is set to “True” by default, which allows you to see the generated email in a nice popup in the admin while the email is being sent. You can deactivate this functionality by changing the setting to “False”.

When you’re ready to customize your email templates, have a look at our tutorials: [Customizing MailBeez Free Email Templates](/documentation/tutorials/customizing-mailbeez-free-email-templates/) and [Customizing MailBeez Premium Email Templates](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)

**Send Copy**  
 This setting tells MailBeez whether or not to send a copy of each email it sends to an email address of your choosing. It is set to “True” by default.

This is a helpful tool when you are customizing your email templates and when you first switch to Production Mode, because it enables you to see and review copies of emails in order to ensure they appear as you expect them to.

When you have completed your customizations and have ensured all is as it should be, you may turn off this functionality by switching the setting to “False”.

**Send Copy To**  
 This field is populated with copy@localhost as an example. Replace it with a valid email address where you would like the email copies sent. It is not necessary to change this field if you have set the “Send Copy” functionality to “False”.

**Max. Number of Copy Emails Sent per MailBeez Module**  
 This setting controls the number of copy emails that MailBeez sends to the email address you listed in the previous setting. It is sent to 10 by default.

When you are first customizing and testing, it may be valuable to enter a high number here to ensure that copies continue to come to you for as long as you need them to. Once testing is completed and all is as it should be in Production Mode, you can go back and change this setting to a lower number, or turn off the functionality altogether by changing the “Send Copy” setting to “False”.

### Security Settings

**Security Token**  
 This setting protects your MailHive, where all of your MailBeez modules and their templates are stored. Unless you are an advanced user, it is recommended that you leave it set at the default value.

### Compatibility Settings

**Popup Mode**  
 This setting allows MailBeez to display certain items in popups inside your admin. For example, this is how email templates are previewed, and also how emails are displayed to you if you have the “Show Email while Sending” setting set to “True”.

It is set to CeeBox by default, but you may turn it off if you are having compatibility issues with CeeBox or simply prefer not to use MailBeez’s preview features.

### Advanced Settings

**Remind to Run Update Check**  
 This setting determines whether or not you will be reminded to check MailBeez and all of your modules for software updates. It is set to “True” by default, but if you prefer not to be reminded to check for software updates, you may turn it off by changing the setting to “False”.

**Enable “Early Check”**  
 Enabling “Early Check” adds an SQL query on a per item, per module basis.

This has the effect of hiding all of the already sent or filtered results, meaning you won’t see these recipients in the Recipients List in your various MailBeez modules.

Some people find this confusing because it will result in seeing a “0 recipients” message in various Recipients Lists if the only recipients are those who have already received this email before (common during testing when you are repeatedly sending to your own email address).

You may want to enable “Early check” temporarily if you need to see a list of recipients from the most recent MailBeez production run. But you won’t want to leave it on all the time, as this slows down your database.

## Simulation Configuration

Simulation settings allow you to control some aspects of the simulation. There is 1 function button and 4 settings to look at here:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://mailbeez.com/images/doc/configuration/config_simulation.png&w=175&h=295&zc=1&q=100 "Simulation Settings")](http://mailbeez.com/images/doc/configuration/config_simulation.png "Simulation Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Control Simulation Options

**Restart Button**  
 Clicking this button will result in all recorded simulation data being deleted, including tracking data.

**Mode**  
 This setting tells MailBeez whether you want to operate in Simulation Mode or Production Mode. It is set to “Simulate” by default, allowing you to explore and play in MailBeez without fear of sending anything out to your customers.  When you’re ready to take MailBeez live, simply change the setting to “Production” to put MailBeez into Production Mode.

**Enable Tracking in Simulation Mode**  
 MailBeez has the ability to track which emails it has sent to which customers, so that customers don’t receive duplicate emails. This setting allows you to enable the tracking feature in Simulation Mode so that you can see how it works.

It is set to “True”, or “On” by default. To turn tracking off, simply change the setting to “False”.

### Control Simulation Emails

**Send Simulation To**  
 This setting tells MailBeez where you want your simulation emails to go. Simply replace “copy@localhost” with a valid email address. All simulation emails will go to this email address for as long as you send emails in simulation mode.

**Send Copy in Simulation Mode**  
 When you edited your “Send Copy to” setting in Basic Configuration Settings, you entered an email address where you want MailBeez to send copies of all outgoing emails.

The “Send Copy in Simulation Mode” setting tells MailBeez whether or not to send simulation mode emails to that email address.

It is set to “True” or “On” by default. If you don’t want copies sent in Simulation Mode, simply turn it off by changing the setting to “False”.

If the email address provided for “Send Copy to” is the same email address provided in the “Send Simulation To” field in the Basic Configuration area, you will get 2 copies of each simulation email you send unless you change this setting to “False”.



## Next Steps

You’re almost there! The last step before you begin testing is to configure the MailBeez modules you wish to test. This is a quick and simple process that can easily be completed in just a couple of minutes.

[Continue to MailBeez Module Configuration tutorials](/documentation/tutorials/mailbeez-tutorials/)

If you have not yet installed any additional modules, you may begin testing with the Birthday Greetings module included with your MailBeez installation, once you [configure it](/documentation/tutorials/birthday-greetings-configuration-tutorial/) of course.

If you prefer to finish configuring MailBeez before proceeding with module configuration, please continue to the [Comprehensive Configuration tutorial.](/documentation/tutorials/mailbeez-comprehensive-configuration-tutorial/) Since you have already completed much of your MailBeez configuration through the Quick Start process, completing configuration should only take a few minutes.
