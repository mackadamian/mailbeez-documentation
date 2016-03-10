---
# http://learn.getgrav.org/content/headers
title: MailBeez Comprehensive Configuration
slug: mailbeez-comprehensive-configuration-tutorial
# menu: MailBeez Comprehensive Configuration
date: 11-07-2012
published: true
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

## Getting Started

Navigate to your MailBeez Dashboard in your store admin and click on the “Configuration” tab. You will see a number of configuration groups, as shown in the screenshot below:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab.png&w=270&h=134&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Each configuration group on the list has a number of configurable settings which can be adjusted to suit your needs, although in most cases, the default settings will serve you best.

In this tutorial, we will go through each configuration group and its associated configurable settings. The entire configuration process can be completed in 15-30 minutes. Let’s get started with the first configuration group on the list: Basic Configuration.

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

## Spam Compliance Configuration

Spam Compliance control is easy with MailBeez! There are only two settings to look at here:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_spam_compliance.png&w=175&h=233&zc=1&q=100 "Spam Compliance Settings")](http://www.mailbeez.com/images/doc/configuration/config_spam_compliance.png "Spam Compliance Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Customer Consent

**Newsletter Subscriber Check**  
 This setting tells MailBeez whether to send emails to all of your customers, or limit emails to only those customers who agreed to be contacted when they created their account.

Setting it to “True” will allow MailBeez to email only those customers who have agreed to be contacted. Leaving it set to “False” will allow MailBeez to send emails to all of your customers. It is set to “False” by default.

In some markets, consent to receive email is implied when the customer creates an account, or when a disclaimer appears on the account creation page. In other markets, customers must actively opt in during account creation to grant consent to receive email. You must set this setting according to your store’s privacy policy and/or your local laws.

If your privacy policy and/or local law is such that only customers who have actively opted in will receive email from you, then you should change this setting to “True”.

### Control Opt-Out Link Behavior

**Opt-Out Link Behavior**  
 This setting allows you to control how customer opt-out requests are handled. It is set to “Module” by default.

This means that the opt-out links in your emails are on a module-by module basis. For example, a customer may click the opt-out link in the Birthday Greeting email, but still continue to receive Review Reminder emails.

If you choose to leave this at the “Module” setting, you may wish to edit the opt-out language in each of your module email templates to something like “Stop sending me \*\*\* emails”, replacing the \*\*\* with the email type (i.e. stop sending me birthday emails, stop sending me review reminder emails, etc). This will make it clear to the customer that they are only opting out of that specific type of email.

Changing this setting to “Global” will cause the customer to be opted out of all MailBeez emails. If you choose to use this setting, you may wish to edit the opt-out language in each of your module email templates to something like “Opt out of all emails from \*\*\*\*”, replacing the \*\*\*\* with your store’s name. This will make it clear to the customer that if they opt out of one, they opt out of all.

Certain modules, such as the Payment Dunning reminder emails will ignore the Newsletter Subscriber Check “True” and Opt-Out Link Behavior “Global” settings. This is because customers who owe you money may not opt out of receiving emails that remind them to make payment.

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

## Email Engine Configuration

If everything in your MailBeez is working as expected, there is no need to make any changes to these settings. Let’s just do a brief overview of the settings so you’ll be familiar with them:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_email_engine.png&w=149&h=396&zc=1&q=100 "Email Engine Settings")](http://www.mailbeez.com/images/doc/configuration/config_email_engine.png "Email Engine Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Select Your Email Template System

**Override Zencart Email Template System**  
**This setting is for Zen Cart users only.** This setting allows you to choose between using Zen Cart’s built in template system, and using the MailBeez template system.

This setting is set to “True” by default, meaning that the MailBeez template system is used. MailBeez templates are editable and may be fully customized with your store graphics and custom content.

Changing this setting to “False” will tell MailBeez to merge its email content into your Zen Cart email templates. If you choose to set this to “False” in order to use your Zen Cart email templates, be aware that if your Zen Cart email templates are highly customized, you may have to do some significant editing in your Zen Cart email template files in order for the MailBeez content to merge in a visually pleasing manner.

For this reason, it is recommended that you leave this setting on “True” unless you are proficient in template design using the html and inline CSS style statements found in Zen Cart email templates. For most users, leaving this setting on “True” is just the easier of the two choices.

**Double Dot Bugfix**  
 On rare occasions a Dot in filenames is doubled, i.e. file.php becomes file..php, image.png becomes image..png. Changing this setting to “True” will attempt to fix that issue. However, the issue is so rare, that it is best to leave this setting off, “False”. You only want to turn this setting to “True” if you are experiencing this issue.

### Email Engine Settings

**Select the Email Engine**  
 This setting allows you to change which email engine you will use to send your MailBeez emails. It is set to “Shop” by default and will use your store’s email engine adhering to the email settings you configured in your store’s email configuration.

You will need to change this setting to PHPMailer v5.2.1 if you are using the [ MailBeez BounceHive Bounce Handling module](/documentation/configbeez/config_bouncehive_advanced/)

The remaining settings only apply if you change your email engine to PHPMailer v5.2.1. These settings are mostly self explanatory, but additional information can be found in the [ MailBeez BounceHive Bounce Handling tutorial](/documentation/tutorials/configbeez-tutorials/-bounce-handling-configuration-tutorial/)

## Dashboard Configuration

These settings allow you to control the layout of the MailBeez Dashboard in your store admin. The Dashboard Configuration Setting has 2 edit buttons on it:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_dash1.png&w=175&h=197&zc=1&q=100 "Dashboard Configuration Settings")](http://www.mailbeez.com/images/doc/configuration/config_dash1.png "Dashboard Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The first edit button allows you to choose which of the first five tabs will be the Start Tab on your MailBeez interface. The default setting is ‘Home’ – i.e. the MailBeez Dashboard:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_dash2.png&w=175&h=136&zc=1&q=100 "Select Dashboard Start Tab")](http://www.mailbeez.com/images/doc/configuration/config_dash2.png "Select Dashboard Start Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The second edit button will take you to an editing screen where you can add, remove, and edit the individual Dashboard Modules in order to customize the layout and look of your MailBeez Dashboard:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_dash3.png&w=270&h=91&zc=1&q=100 "Edit Dashboard Modules")](http://www.mailbeez.com/images/doc/configuration/config_dash3.png "Edit Dashboard Modules")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

With MailBeez, you are in control. You decide which data is important to you, what you want to see, and how you want to see it!

## Event Log Configuration

These settings allow you to choose which events you would like to log when MailBeez is run. This information is useful for both monitoring the run and for troubleshooting the issue in the event of a problem.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_event_log.png&w=175&h=105&zc=1&q=100 "Event Log Settings")](http://www.mailbeez.com/images/doc/configuration/config_event_log.png "Event Log Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The speed at which emails are processed and sent out is slightly lowered when logging is on, but the speed difference is very minimal and is far outweighed by the benefits of logging. It is recommended that both settings be activated.

**MODULE\_INIT**  
 Activate this setting by clicking on the checkbox. This setting logs the initialization of modules when they are run. When this setting is activated, you will see the following message in your log file if the initialization of the module(s) was without incident:

MAILHIVE\_RUN\_INIT: MailBeez is started

**MODULE\_SQL**  
 Activate this setting by clicking on the checkbox. This setting logs the sql query of modules when they are run. When this setting is activated, you will see the following message in your log file if the run of the module(s) was without incident:

MAILHIVE\_RUN\_COMPLETE: MailBeez has finalized successfully

Ideally, you want to see both of these success messages in your log files. Log files may be accessed at Admin > MailBeez > Reports > MailBeez Event Log Viewer. If something does go wrong and you need assistance interpreting error messages in your log files, please use our Live Chat feature to reach out to us.

## MailHive Process Control Configuration

These settings are for advanced users, so you should leave them as they are unless you know what you’re doing.

## Google Analytics Integration

**Google Analytics Integration settings need to be configured only if you have a Google Analytics account.**

There are 5 configurable settings in the Google Analytics Automatic Campaign Integration configuration:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_ga.png&w=175&h=258&zc=1&q=100 "Google Analytics Settings")](http://www.mailbeez.com/images/doc/configuration/config_ga.png "Google Analytics Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Google Analytics Settings

**Google Analytics Integration**  
 This setting turns Google Analytics integration on and off. It is set to “True” by default. It operates on a global basis, meaning that Google Analytics integration is either on or off for all of your MailBeez modules.

**Google Analytics URL Rewrite Mode**  
 This setting lets you choose which of your URLs will be rewritten to include Google Analytics code so that link clicks can be tracked and recorded in your Google Analytics account.

If you choose “shop”, only links to your shop will be tracked when clicked. If you choose “all”, all links will be tracked when clicked. It is set to “all” by default.

This setting is global, meaning that all of your MailBeez modules are affected by this setting; however you can disable URL rewriting in specific email templates by disabling the generated email link either in the email template or in the email text. You do this by inserting a blank space into the href statement in the anchor tag:

 
    <pre class="fancy_pre_box">
    Example: [html]<a href=”http://www.mailbeez.com">This link will be rewritten</a>[/html]
    Example: [html]<a href = “http://www.mailbeez.com">This link will NOT be rewritten due to spaces inserted before and after the = sign</a>[/html]


**Google Analytics URL Rewrite in TXT Format**  
 This setting ensures that your URLs are rewritten for tracking even in text only emails. It is set to “True” by default. If you change it to “False”, email links in text only emails will not be tracked.

### Google Analytics Report Data Settings

**Google Analytics “Medium”**  
 This setting allows you to change the name of the medium through which the link click data came to Google Analytics. It is set to “email” by default.

When you look at your Google Analytics reports, you will see the link click data collected through the email medium. This helps you differentiate between link clicks coming from a site where you have paid advertising vs. those coming from your own customer emails. If you’re getting more clicks through your free emails than through paid advertising, then it may be time to re-allocate your advertising dollars. In other words, using MailBeez can help you determine where best to invest your advertising budget!

**Google Analytics “Source”**  
 This setting allows you to choose the “Source” for Google Analytics. It is set to “MailBeez” by default. This setting works with the “Medium” setting above by helping you determine which email data in your Google Analytics reports came from MailBeez email campaigns vs. other non-MailBeez email campaigns you may be running, like a monthly specials email.

## MailBeez Analytics Settings

### How MailBeez Analytics Can Help Your Business

Before we get to how to configure MailBeez Analytics, let’s talk about what it is and how it works. MailBeez Analytics allows you to track:

- Opening of Emails (Html with loaded images)
- Clicks on Links
- Purchases following clicks on email links

The Open Rates are measured in two ways:

- When tracker images are loaded, this is logged as an opened email
- When a link in an email is clicked on, this is counted as an opened email

The tracker images use a high-performance call to minimize server load: each opening is logged into a log-file. With every run of MailHive, the server handler is importing the log file into the MailBeez Tracking Database. Afterwards, the log file is deleted.

Opens and Clicks On ‘copy to’ emails are not counted because these emails are separate emails with a different message-id. This prevents the tracking from counting your administrative copies and thereby keeping your tracking count pure.

### Installing MailBeez Analytics

Using direct user tracking can be against the law in your country. You are responsible for using MailBeez in compliance with the law.

1. Navigate to your MailBeez interface in your store’s admin
2. Click on the Configuration tab
3. Scroll down to MailBeez Analytics and click on it. You will see this:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_mb_analytics1.png&w=175&h=191&zc=1&q=100 "MailBeez Analytics Activation")](http://www.mailbeez.com/images/doc/configuration/config_mb_analytics1.png "MailBeez Analytics Activation")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Click on the Activate User Tracking button
2. You will see this popup:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_mb_analytics2.png&w=175&h=123&zc=1&q=100 "User Tracking Activation")](http://www.mailbeez.com/images/doc/configuration/config_mb_analytics2.png "User Tracking Activation")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Copy the code from the popup and leave the popup open
2. Download this file to your local drive (your computer) from your server:
 

    <pre class="fancy_pre_box"> Your_Store/includes/application_top.php

1. Paste the code you just copied from the popup at the end of the file before the closing ?>PHP tag
2. Save the file and upload it back to your server
3. Return to your store admin and click the “Activate User Tracking” button in the popup.
4. If you had already closed the popup, click the “Activate User Tracking” button in the
5. MailBeez Analytics settings to bring the popup back, and then click the “Activate User
6. Tracking” button within the popup.
7. You will be redirected back to the MailBeez Dashboard.
8. Navigate back to the Configuration Tab and click on MailBeez Analytics.

The settings pane now looks like this:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configuration/config_mb_analytics3.png&w=175&h=276&zc=1&q=100 "MailBeez Analytics Settings")](http://www.mailbeez.com/images/doc/configuration/config_mb_analytics3.png "MailBeez Analytics Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Configuring MailBeez Analytics

There are 6 configurable settings to look at, as indicated in the screenshot above. Let’s go through them one at a time.

**Enable MailBeez Analytics**  
 This setting turns MailBeez Analytics off and on. By default, it is turned on – “True”. If you ever need to turn MailBeez Analytics off, simply change this setting to “False”. You can ignore the prompt at the top to insert code into the application\_top.php file because you already did that during the installation steps you just completed.

**Real-Time Open Rates**  
 This setting tells MailBeez to refresh your open rates data every 30 seconds. It is set to “True” by default. If you are running a high-load site (i.e. you process a lot of emails to a lot of customers and they are all opening them), then change this setting to “False” and set up a cronjob to manage this for you. Otherwise, your site will be slowed down significantly.

**Process MailBeez Analytics Information With Every Run of MailHive**  
 This setting tells MailBeez whether or not to run MailBeez Analytics every time MailHive is run (i.e. every time a batch of outgoing emails is processed). It is set to “True” by default.

If you choose to change this setting to “False”, you will need to do one of the following in order to process your MailBeez Analytics data:

- Manually run the Service Handler for MailBeez Analytics module, or
- Set up a dedicated cronjob to do it for you automatically, or
- [Install the Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)

The Service Handler for MailBeez Analytics module is located in the MailBeez interface in the MailBeez Modules tab.

The Service Handler for MailBeez Analytics module will be invisible in the MailBeez Modules tab unless this setting is set to “False”.

**Insert Tracking Pix Automatically**  
 This setting tells MailBeez whether or not to automatically insert Tracking Pix to the end of your module body content. It is set to “True” by default. If this causes design layout issues, change the setting to “False” and manually insert the Tracking Tag provided into your Main Template before the closing body tag.

**Add Click-Tracking to URLs in TXT Format?**  
 This setting gives you the option to add Click-Tracking to URLs in text only emails. It is set to “True” by default. If you change the setting to false, email links included in text only emails will not be tracked.

**Rows per Page**  
 This setting controls how many rows of MailBeez Analytics data are displayed per page.

## Template Engine

Leave these settings as they are.

The “Clear” button will clear your cached templates. This function is is to be used after you’ve made changes to configurations outside of MailBeez (like a change to an already configured cron-job, for example), or if there is an issue with the template engine.

## Remaining Configuration Options

The remaining configuration options are all additional configuration modules which bring value added services to your ecommerce experience and are available for purchase on the **[ MailBeez website.](http://www.mailbeez.com/download/)**

- Bounce Handling
- Email Throttling
- Run MailBeez Automatically
- Template Manager

**[ Bounce Handling](/documentation/configbeez/config_bouncehive_advanced/)**  
 Bounced emails add an extra level of unnecessary work for shop owners. Every time an email bounces, you must edit your email lists to ensure their removal. In a large shop, this can be a nightmarish experience. Too many bounced emails can get your account flagged as a spam sender and cause problems with your hosting account.

This configuration module puts an end to all that by automatically managing your bounced emails. If an email bounces, Bounce Handling will mark the customer accordingly and avoid sending out additional emails.

**[Email Throttling](/documentation/mailbeez/filter_do_throttling_simple/)**  
 MailBeez Simple Throttling module is a simple, yet highly useful filter that allows you to configure the hourly rate and total number of emails that MailBeez sends out.

Once you start firing off a lot of emails, it’s a good idea to consider working with email throttling. Whether your store runs on a limited data plan involving hourly email restrictions, or you simply want to make sure that your site is still responsive to visitors even whilst the server fires off emails behind the scenes, email throttling is key, and the Mailbeez Simple Throttling module is the tool to use to achieve it.

**[Run MailBeez Automatically](/documentation/configbeez/config_cron_simple/)**  
 If you want MailBeez to run automatically, you have two options. You may either:

- Set up a cronjob to manage the automation for you
- Install the simple and affordable Run MailBeez Automatically module

Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for many users by far the easier of the two options.

**[Template Manager](/documentation/configbeez/config_tmplmngr/)**  
 Mailbeez has developed a handy module that easily allows you to both edit and view your text changes right from the MailBeez interface within your store’s admin. Fully functional with all official (free and premium) MailBeez Modules as well as with custom built modules, the Mailbeez Template Manager makes editing a template a breeze, so much so that you may wonder how you ever lived without it!

**[Mouseflow](/documentation/configbeez/config_mouseflow/)**  
 Mouseflow is a third party web service which can be easily and affordably be fully integrated into your MailBeez installation with the MailBeez Mouseflow Integration module. Mouseflow gathers data, telling you which areas of your site are getting the most attention by your visitors. Areas being overlooked by users can then be improved to gain more attention.

Furthermore Mouseflow can actually record a visitor’s activity on your site. This can greatly help you in determining the user friendliness of the site and how visitors interact with the available tools.



## Next Steps

You’re almost there! The last step before you begin testing is to configure the MailBeez modules you wish to test. This is a quick and simple process that can easily be completed in just a couple of minutes.

 If you have not yet installed any additional modules, you can begin testing with the Birthday Greetings module included with your MailBeez installation, once you [configure it](/documentation/tutorials/birthday-greetings-configuration-tutorial/) of course.
