---
# http://learn.getgrav.org/content/headers
title: Pattern Blacklist
slug: ID-4738
# menu: Pattern Blacklist
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

The screenshots used in this tutorial were made using Zen Cart. If you use a different e-commerce platform, your admin interface and MailBeez interface may appear slightly different, however the concepts and configuration instructions are the same across all platforms.

 

## About This Module

This handy Mailbeez module gives you the tools to set up an email blacklist based on email address patterns that you define. A good example of its usefulness is that you could create a blacklist to block MailBeez for all customers created through a store integration with Amazon. Pattern Blacklist allows you to define an unlimited number of patterns.  
  

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Filter & Helper tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/filter_tab.png&w=270&h=85&zc=1&q=100 "Filter & Helper Tab")](http://www.mailbeez.com/images/doc/common_images/filter_tab.png "Filter & Helper Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Pattern Blacklist module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_check_pattern_blacklist/pattern_blacklist_config1.png&w=175&h=81&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/filterbeez/filter_check_pattern_blacklist/pattern_blacklist_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration settings are now available for you to edit:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_check_pattern_blacklist/pattern_blacklist_config2.png&w=175&h=255&zc=1&q=100 "Pattern Blacklist Configuration Settings")](http://www.mailbeez.com/images/doc/filterbeez/filter_check_pattern_blacklist/pattern_blacklist_config2.png "Pattern Blacklist Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring the Pattern Blacklist Module

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on second “Edit” button at the bottom of the configuration panel
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready for configuration.

### Configure General Settings

Click the “Edit” button to access the general settings. There are 2 of them:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_check_pattern_blacklist/pattern_blacklist_config3.png&w=175&h=236&zc=1&q=100 "Pattern Blacklist General Settings")](http://www.mailbeez.com/images/doc/filterbeez/filter_check_pattern_blacklist/pattern_blacklist_config3.png "Pattern Blacklist General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “True” by default, meaning the module is on and ready to work. Change this setting to “False” to deactivate the module and disable it from being run.

**Blacklist Pattern**  
 This setting lets you define the email address patterns you wish to block. For example, if you have a store on Amazon that is integrated with your main store, you might want to block MailBeez from sending emails to accounts created via that integration. You would do this by entering this email address pattern: @marketplace.amazon.com

There is no limit to the number of patterns you can write. Simply enter one pattern per line, no commas or semi-colons are required to separate the lines.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.
