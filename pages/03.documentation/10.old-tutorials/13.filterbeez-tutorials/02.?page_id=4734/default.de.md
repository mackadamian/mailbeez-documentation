---
# http://learn.getgrav.org/content/headers
title: Add Gender
slug: ID-4734
# menu: Add Gender
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

This module adds gender information to all of your MailBeez email modules and allows you to email your customers on a gender specific basis, resulting in a higher degree of reader relevancy and making customers less likely to unsubscribe for receiving emails about products that don’t interest them.  
  

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Filter & Helper tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/filter_tab.png&w=270&h=85&zc=1&q=100 "Filter & Helper Tab")](http://www.mailbeez.com/images/doc/common_images/filter_tab.png "Filter & Helper Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Add Gender module and click on it.
5. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_add_gender/add_gender_config1.png&w=175&h=249&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/filterbeez/filter_add_gender/add_gender_config1.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration settings are now available for you to edit:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_add_gender/add_gender_config2.png&w=175&h=374&zc=1&q=100 "Add Gender Configuration Panel")](http://www.mailbeez.com/images/doc/filterbeez/filter_add_gender/add_gender_config2.png "Add Gender Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring the Add Gender Module

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on second “Edit” button at the bottom of the configuration panel
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready to work once you edit your email template files.

### Configure General Settings

Since the Add Gender module is already activated by default, no further configuration of the module is necessary. If you need to deactivate the module for any reason, navigate to MailBeez > Filter & Helper tab > Add Gender Content, the topmost “Edit” button, and change the setting to “False”.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/filterbeez/filter_add_gender/add_gender_config3.png&w=175&h=101&zc=1&q=100 "Add Gender General Settings")](http://www.mailbeez.com/images/doc/filterbeez/filter_add_gender/add_gender_config3.png "Add Gender General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## How Do I Use It?

Below are some examples that demonstrate how to develop gender specific content in the MailBeez template files. You can copy and paste it into your email template files, or use it to get you started creating gender specific content of your own.

### Create a Gender Specific Salutation

Adding this bit of code to your email templates will result in female customers being addressed as “Mrs. Last Name”, male customers being addressed as “Mr Last Name”, and customers of unknown gender as “First Name Last Name”.

{if $gender == “f”}  
 Dear Mrs. {$lastname}  
 {elseif $gender == “m”}  
 Dear Mr. {$lastname}  
 {else}  
 Hello {$firstname} {$lastname}  
 {/if}

### Include Gender Specific Salutation in the Subject Line

To include a gender specific salutation in your email subject lines, take the above code and add it to your template in a single line.

{if $gender == “f”} Dear Mrs. {$lastname} {elseif $gender == “m”} Dear Mr. {$lastname} {else} Hello {$firstname} {$lastname} {/if}

### Include Gender Specific Language in Email Content

Create email campaigns for gender specific products that target customers by gender and use gender specific language within the email.

{if $gender == “f”}  
 Sample Text: Pamper yourself with these luxurious bath products!  
 {elseif $gender == “m”}  
 Sample Text: Your next barbecue will be a hit with one of these awesome grills!  
 {else}  
 Sample Text: Great gifts for everyone!  
 {/if}  
  

## How Do I Edit My Email Templates?

You do need to be able to customize your MailBeez templates to utilize this add on, so if you do not feel confident making these edits yourself, or feel you do not have enough experience with this, you can [get some professional MailBeez support](http://www.mailbeez.com/support/service/) or have a look at our tutorial on [Customizing MailBeez Premium Email Templates](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.
