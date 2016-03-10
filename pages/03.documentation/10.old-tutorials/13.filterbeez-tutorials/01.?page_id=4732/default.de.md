---
# http://learn.getgrav.org/content/headers
title: Simple Throttling
slug: ID-4732
# menu: Simple Throttling
date: 22-07-2012
published: false
publish_date: 22-07-2012
# unpublish_date: 22-07-2012
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

Simple Throttling allows you to configure the hourly rate and total number of emails that MailBeez sends out. This is useful because many hosting companies place a limit on how many emails can be sent out at once and in total. Accounts exceeding those limits can trigger automatic spam alerts that hosting companies have in place to protect their servers.

Simple Throttling keeps you in good standing with your hosting company and helps you ensure that your site is still responsive to visitors while the server fires off emails behind the scenes.  
  

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Filter & Helper tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/filter_tab.png&w=270&h=85&zc=1&q=100 "Filter & Helper Tab")](http://www.mailbeez.com/images/doc/common_images/filter_tab.png "Filter & Helper Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Simple Throttling module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_do_throttling_simple/simple_throttling_config1.png&w=175&h=80&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/filterbeez/filter_do_throttling_simple/simple_throttling_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration settings are now available for you to edit:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_do_throttling_simple/simple_throttling_config2.png&w=175&h=270&zc=1&q=100 "Simple Throttling Configuration Settings")](http://www.mailbeez.com/images/doc/filterbeez/filter_do_throttling_simple/simple_throttling_config2.png "Simple Throttling Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring the Simple Throttling Module

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on second “Edit” button at the bottom of the configuration panel
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready for configuration.

### Configure General Settings

Click the “Edit” button to access the general settings. There are 3 of them:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_do_throttling_simple/simple_throttling_config3.png&w=175&h=185&zc=1&q=100 "Simple Throttling General Settings")](http://www.mailbeez.com/images/doc/filterbeez/filter_do_throttling_simple/simple_throttling_config3.png "Simple Throttling General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “True” by default, meaning the module is on and ready to work. Change this setting to “False” to deactivate the module and disable it from being run.

**Emails Per Hour**  
 This setting lets you control the rate per hour at which MailBeez is sending emails. By default it is set to 480, but you should check with your hosting company to find out what your limit is and set this number accordingly.

**Maximum Number of Emails per Run**  
 This setting lets you control the maximum number of emails that will be sent out in a single run. It is set to 2000 by default, but you should contact your hosting company to find out what your limit is and, taking into consideration the size of your mailing list, set this number accordingly.

Once either of these limits are hit, Simple Throttling waits for the next cron job cycle before sending out the remaining emails.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.
