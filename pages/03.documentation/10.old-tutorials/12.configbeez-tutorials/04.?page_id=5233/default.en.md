---
# http://learn.getgrav.org/content/headers
title: Mouseflow Integration
slug: ID-5233
# menu: Mouseflow Integration
date: 07-08-2012
published: false
publish_date: 07-08-2012
# unpublish_date: 07-08-2012
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

[Mouseflow](http://localhost/wordpress_mailbeez_EOL/wp-content/plugins/adrotate/adrotate-out.php?track=OSwwLDAsaHR0cDovL3d3dy5zaGFyZWFzYWxlLmNvbS9yLmNmbT9iPTIyOTA5NiZhbXA7dT00NTAwNjEmYW1wO209MjcxODImYW1wO3VybGxpbms9JmFtcDthZmZ0cmFjaz0) is a web service that gathers data, telling us which areas of our site are getting the most attention by our visitors. Areas being overlooked by users can then be improved to gain more attention.

The MailBeez Mouseflow Integration module works with your existing Mouseflow installation to allow you to track visitors arriving to your site from links within all of your MailBeez generated emails.

To use this module, you must already have a [Mouseflow](http://localhost/wordpress_mailbeez_EOL/wp-content/plugins/adrotate/adrotate-out.php?track=OSwwLDAsaHR0cDovL3d3dy5zaGFyZWFzYWxlLmNvbS9yLmNmbT9iPTIyOTA5NiZhbXA7dT00NTAwNjEmYW1wO209MjcxODImYW1wO3VybGxpbms9JmFtcDthZmZ0cmFjaz0) account set up and installed on your website.

Installation and configuration are fast and easy! Installation instructions are included in the download package. Configuration instructions are below.

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Configuration tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab2.png&w=270&h=175&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab2.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Mouseflow Integration module and click on it.
5. Click on the Install button to install the configuration settings into your database:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_mouseflow/install.png&w=175&h=130&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/configbeez/config_mouseflow/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_mouseflow/config_mouseflow.png&w=175&h=324&zc=1&q=100 "Mouseflow Integration Configuration Settings")](http://www.mailbeez.com/images/doc/configbeez/config_mouseflow/config_mouseflow.png "Mouseflow Integration Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring the Module

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on second “Edit” button at the bottom of the configuration panel
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

   
 Your module is now unlocked and ready for configuration.

### Configure General Settings

Click the top-most “Edit” button to access the general settings. There are 4 of them:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_mouseflow/general_settings.png&w=175&h=394&zc=1&q=100 "Mouseflow Integration General Settings")](http://www.mailbeez.com/images/doc/configbeez/config_mouseflow/general_settings.png "Mouseflow Integration General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “True” by default, meaning the module is on and ready to work. Change this setting to “False” to deactivate the module and disable it from being run.

**Mouseflow Recording is Active For**  
 This setting lets you define which channel you would like to record for. Do you want to record only those visits that are generated by the links in your MailBeez generated emails, or do you want to record all visits to your store? By default, it is set to MailBeez in order to help you track which email links are generating traffic as well as the activity resulting from that traffic whilst minimize the number of recordings for your Mouseflow account.

This is extremely useful if you’ve signed up for a free or budget-conscious [Mouseflow](http://localhost/wordpress_mailbeez_EOL/wp-content/plugins/adrotate/adrotate-out.php?track=OSwwLDAsaHR0cDovL3d3dy5zaGFyZWFzYWxlLmNvbS9yLmNmbT9iPTIyOTA5NiZhbXA7dT00NTAwNjEmYW1wO209MjcxODImYW1wO3VybGxpbms9JmFtcDthZmZ0cmFjaz0) account. However, if you’ve opted to have a larger account with Mouseflow and want to track everything, you can change this setting to “Other”.

**Exclude Visitors Based on IP Address**  
 This setting allows you to exclude the tracking of visitors based on their IP address. For example, you won’t want to include your own browsing of your website in your statistics. Additionally, you may have business partners or employees who’s visits and browsing behavior does not need to be tracked.

It is up to you who to exclude from tracking, but you want to keep in mind that your [Mouseflow](http://localhost/wordpress_mailbeez_EOL/wp-content/plugins/adrotate/adrotate-out.php?track=OSwwLDAsaHR0cDovL3d3dy5zaGFyZWFzYWxlLmNvbS9yLmNmbT9iPTIyOTA5NiZhbXA7dT00NTAwNjEmYW1wO209MjcxODImYW1wO3VybGxpbms9JmFtcDthZmZ0cmFjaz0) account has a limit of tracings and recordings allowed, so if you have decided to begin with a free or budget-conscious option, you will definitely want to exclude anyone who’s visits you don’t care about tracking.

The IP addresses provided here are examples only. Remove them and replace them with the IP addresses of your choosing. For your convenience, your own IP address is displayed beneath the box to help you get started. Simply copy and paste it in.

**Your Mouseflow Code**  
 When you log in to your [Mouseflow](http://localhost/wordpress_mailbeez_EOL/wp-content/plugins/adrotate/adrotate-out.php?track=OSwwLDAsaHR0cDovL3d3dy5zaGFyZWFzYWxlLmNvbS9yLmNmbT9iPTIyOTA5NiZhbXA7dT00NTAwNjEmYW1wO209MjcxODImYW1wO3VybGxpbms9JmFtcDthZmZ0cmFjaz0) account and go to your admin area, you will see a code. Simply copy that code, return here, and paste it in. Click the “Update” button and move on to the next step.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!

 

## The Mouseflow Integration Filter

You may ignore this filter as mouseflow is now pre-integrated into mailbeez and becomes active when the Mouseflow module is installed and activated.

There is nothing more you need to do. This module is fully automated, so you should start seeing report statistics in your [Mouseflow](http://localhost/wordpress_mailbeez_EOL/wp-content/plugins/adrotate/adrotate-out.php?track=OSwwLDAsaHR0cDovL3d3dy5zaGFyZWFzYWxlLmNvbS9yLmNmbT9iPTIyOTA5NiZhbXA7dT00NTAwNjEmYW1wO209MjcxODImYW1wO3VybGxpbms9JmFtcDthZmZ0cmFjaz0) admin soon after the next run of your email modules!
