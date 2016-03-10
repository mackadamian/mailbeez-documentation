---
# http://learn.getgrav.org/content/headers
title: Customer Group Filter
slug: ID-5281
# menu: Customer Group Filter
date: 08-08-2012
published: false
publish_date: 08-08-2012
# unpublish_date: 08-08-2012
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

**Please Note: This module is Zen Cart, CRE Loaded B2B, xt:Commerce, xtc-Modified and Gambio GX compliant only.**

If you sell to different customer groups, then the Customer Group Filter is for you! This handy module allows you to choose which customer groups will receive your various Mailbeez campaigns.

Since different market sectors will almost certainly have individual marketing needs, splitting customers into groups is a great idea! For example, you probably don’t want a wholesale customer to receive a product review request, or an end user customer to receive a product offer at the wholesale price. The Mailbeez Group Filter module gives you the ability to choose which group is authorized to receive a campaign.  
  

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Filter & Helper tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/filter_tab.png&w=270&h=85&zc=1&q=100 "Filter & Helper Tab")](http://www.mailbeez.com/images/doc/common_images/filter_tab.png "Filter & Helper Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Customer Group Filter module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config1.png&w=175&h=82&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration settings are now available for you to edit:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config2.png&w=175&h=270&zc=1&q=100 "Customer Group Filter Configuration Settings")](http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config2.png "Customer Group Filter Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

## Configuring the Customer Group Filter Module

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on the second “Edit” button at the bottom of the configuration panel.
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready for configuration:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config3.png&w=175&h=266&zc=1&q=100 "Customer Group Filter Configuration Panel")](http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config3.png "Customer Group Filter Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Configure Customer Groups

1. Click the “Configure” button in the center of the configuration panel, as shown in the image above.
2. If you have not yet created customer groups in your store, you will see this:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config4.png&w=270&h=129&zc=1&q=100 "Unconfigured Customer Groups Panel")](http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config4.png "Unconfigured Customer Groups Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Note that in the image above, the only customer group is “Default Group”. This is the group all customers are in unless and until you assign them to another customer group.

Note also that there are no MailBeez modules assigned to the default group. MailBeez does not automatically assign any customer groups to your email campaign modules, allowing you complete freedom and flexibility to decide which groups will receive which email campaigns.

6. If you have not yet created customer groups in your store, do so now. Each e-commerce platform has its own process for creating customer groups. Please refer to your e-commerce platform’s documentation for instructions on how to create customer groups.
7. Once you have created your customer groups, navigate back to MailBeez > Filter & Helper tab > Customer Group Filter and click the “Configure” button.
8. Assign customer groups to various MailBeez email modules by clicking the check boxes. You can click as many or as few customer groups as you like for each module. Remember that the Default Group = all customers not assigned to any customer group.
9. Once you have created your customer groups and assigned them to the MailBeez email modules of your choice, you will see this:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config5.png&w=270&h=129&zc=1&q=100 "Configured Customer Groups Panel")](http://www.mailbeez.com/images/doc/filterbeez/filter_check_group/customer_group_filter_config5.png "Configured Customer Groups Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


Since the Customer Groups Filter module is already activated by default, your Customer Groups Filter module is now configured and ready to work! If you need to deactivate the module for any reason, navigate to MailBeez > Filter & Helper tab > Customer Group Filter, the topmost “Edit” button, and change the setting to “False”.



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.
