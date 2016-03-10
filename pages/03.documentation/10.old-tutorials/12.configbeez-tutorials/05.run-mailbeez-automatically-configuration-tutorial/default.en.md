---
# http://learn.getgrav.org/content/headers
title: Run MailBeez Automatically
slug: run-mailbeez-automatically-configuration-tutorial
# menu: Run MailBeez Automatically
date: 07-08-2012
published: true
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

With this simple Mailbeez add-on, you can do away with the need to configure a cronjob to activate your Mailbeez installed modules. Instead, the plugin cleverly utilizes your store’s traffic to trigger Mailbeez as often as you have configured it to run. For site owners looking to get up and running quickly, or who do not wish to enter the server environment to setup a Cronjob, this is a very handy feature.

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Configuration tab

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab2.png&w=270&h=175&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab2.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Locate the Run MailBeez Automatically – Simple Cronjob module and click on it.
2. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_cron_simple/cron_simple_config1.png&w=175&h=179&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/configbeez/config_cron_simple/cron_simple_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_cron_simple/cron_simple_config2.png&w=175&h=313&zc=1&q=100 "Run MailBeez Automatically Configuration Settings")](http://www.mailbeez.com/images/doc/configbeez/config_cron_simple/cron_simple_config2.png "Run MailBeez Automatically Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

## Configuring the Module

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on second “Edit” button at the bottom of the configuration panel
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready for configuration.

### Configure General Settings

Click the top-most “Edit” button to access the general settings. There are 2 of them:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_cron_simple/cron_simple_config3.png&w=175&h=135&zc=1&q=100 "Run MailBeez Automatically General Settings")](http://www.mailbeez.com/images/doc/configbeez/config_cron_simple/cron_simple_config3.png "Run MailBeez Automatically General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “True” by default, meaning the module is on and ready to work. Change this setting to “False” to deactivate the module and disable it from being run.

**Time Between Running MailBeez (hours)**  
 This setting lets you control the amount of time in hours between MailBeez runs. By default, it is set to 24 hours meaning that MailBeez will wait 24 hours after a run is completed before starting the next run.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!
