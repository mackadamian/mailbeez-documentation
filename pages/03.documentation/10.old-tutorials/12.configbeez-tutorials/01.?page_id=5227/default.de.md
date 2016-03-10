---
# http://learn.getgrav.org/content/headers
title: Advanced Opt-Out with Admin
slug: ID-5227
# menu: Advanced Opt-Out with Admin
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

(English)

The screenshots used in this tutorial were made using Zen Cart. If you use a different e-commerce platform, your admin interface and MailBeez interface may appear slightly different, however the concepts and configuration instructions are the same across all platforms.

## About This Module

This module enhances the default Opt-Out handling which is already built into MailBeez by allowing you to adjust customer Opt-Out settings by manually editing which of your customers will receive Mailbeez generated emails. And it can all be done from within your store’s admin! With this module, you can:

- Insert “block all” links into your email templates, allowing customers to choose between blocking specific emails and blocking all MailBeez generated emails
- Manually unblock customers who opt-out via accidental click
- Disable opt-out for selected modules – for example, payment reminder emails
- Manually block and unblock a customer on a per module basis
- Manually block and unblock a customer on a global basis

 

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Configuration tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab2.png&w=270&h=175&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab2.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Opt-Out/Block Administration module and click on it.
5. Click on the Install button to install the configuration settings into your database:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/install.png&w=175&h=81&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/config_panel_locked.png&w=175&h=224&zc=1&q=100 "Advanced Opt-Out with Admin Configuration Settings")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/config_panel_locked.png "Advanced Opt-Out with Admin Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring the Module

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on second “Edit” button at the bottom of the configuration panel
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

   
 Your module is now unlocked and ready for configuration:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/config_panel_unlocked.png&w=175&h=314&zc=1&q=100 "Advanced Opt-Out with Admin Configuration Settings")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/config_panel_unlocked.png "Advanced Opt-Out with Admin Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Configure General Settings

Click the top-most “Edit” button to access the general settings. There are 2 of them:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/general_settings.png&w=175&h=114&zc=1&q=100 "Advanced Opt-Out with Admin General Settings")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/general_settings.png "Advanced Opt-Out with Admin General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Hide Helper Modules**  
 This setting is set to “False” by default, meaning that the helper modules used by the Advanced Opt-Out with Admin module are visible in the MailBeez interface.

The helper modules do not have configuration settings and are all internal services that Advanced Opt-Out with Admin uses to manage your “Block All” and “Opt-Out” requests. There is no reason they need to be shown in the MailBeez interface; it is purely a matter of personal preference.

Therefore you may safely change this setting to “True” if you prefer to hide the helper modules from the MailBeez interface. For those who are curious about what the helper modules do, more information is provided below.

The Advanced Opt-Out with Admin module installs and uses the following helper modules:

*Service: Block All Handler*, found in the MailBeez Modules tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/helper_service.png&w=270&h=108&zc=1&q=100 "Service: Block All Handler helper module")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/helper_service.png "Service: Block All Handler helper module")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

This is an internal service that Advanced Opt-Out with Admin uses to capture “Block All” requests.

*Block Customer Administration Check* and *Add Block All Link*, found in the Filter & Helper tab:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/helper_filters.png&w=270&h=41&zc=1&q=100 "Helper Filter Modules")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/helper_filters.png "Helper Filter Modules")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

When a MailBeez email module is run, the *Block Customer Administration Check* filter looks to see if any customers who would normally get that email are on your block list and prevents the module from sending them an email. If the module being run is in your Exclusions list, this filter will be overridden and the email will be sent out.

When you look at this filter, you will see it offers a search option so you can find customers to block and unblock:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/block_customer_check_filter.png&w=175&h=155&zc=1&q=100 "Block Customer Check Filter")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/block_customer_check_filter.png "Block Customer Check Filter")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

However, this same option is available in the Advanced Opt-Out with Admin configuration panel as well as the Opt-Out Dashboard Widget, so if you choose to hide your helper modules, you may do so without losing any functionality.

The *Add Block All Link* – Once you have inserted a “Block All” link to your email templates, then anytime a MailBeez email module is run this filter looks to see if any customers who would normally get that email have clicked the link previously. The filter then prevents the module from sending them an email. If the module being run is in your Exclusions list, this filter will be overridden and the email will be sent out.

**Sort Order of Display**  
 This setting allows you to change the sort order of this module to move it higher or lower on the list of modules in the Configuration tab.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!

 

## Installing the Opt-Out Dashboard Widget

Installing the Opt-Out Dashboard widget is entirely optional, but we think you’ll find this widget so handy that once you have it installed, you’ll never want to give it up!

1. While still in the Configuration tab of the MailBeez interface, navigate to Dashboard Configuration
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install1.png&w=270&h=54&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install1.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click on the 2nd “Edit” button at the bottom of the configuration panel
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install2.png&w=175&h=176&zc=1&q=100 "Dashboard Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install2.png "Dashboard Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. Locate the Customer Opt-Out Admin module and click on it to expose the installation panel
6. Click on the “Install” button to install the dashboard widget’s configuration settings into your database
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install3.png&w=175&h=79&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install3.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

8. The module is already active, so the only configuration necessary is if you want to change the widget’s sort order
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install4.png&w=175&h=154&zc=1&q=100 "Opt-Out Widget Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install4.png "Opt-Out Widget Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

10. Click the “Back to Dashboard” button in the upper left corner to return to the dashboard and view the widget
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install5.png&w=270&h=94&zc=1&q=100 "Opt-Out Customer Admin Widget")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/widget_install5.png "Opt-Out Customer Admin Widget")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


 

## How Do I Use Advanced Opt-Out with Admin?

In this section, we’ll take you step-by-step through all of the ways in which you can use this module to increase the flexibility and control of your customer opt-out settings:

- Disable opt-out for selected modules
- Block & unblock customers globally or per-module
- Allow customers to choose which modules to opt-out of, thereby reducing your global opt-outs

### Disable Opt-Out for Selected Modules

You will want to use this feature judiciously. It can be dangerous to your business to disable the customer’s ability to opt-out of receiving emails. In an age of social media, the last thing you want to do is make customers angry by taking away their right to opt-out. There is also the matter of legality, which varies by location. You are responsible to ensure you are following the laws of your state and country.

Having said that, there are times when it is quite appropriate to disable the customer’s ability to opt-out of receiving emails. For example, if a customer owes you money, you don’t want them to be able to opt out of receiving payment reminders and debt-collection emails.

There are two steps to disabling a module’s opt-out ability:

#### Assign Modules to Exempt List

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Configuration tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab2.png&w=270&h=175&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab2.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Opt-Out/Block Administration module and click on it.
5. Click on the “Exception List” button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/exception_list_button.png&w=175&h=47&zc=1&q=100 "Exception List")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/exception_list_button.png "Exception List")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

7. The Exception List Administration panel is now visible:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/exception_list_administration.png&w=270&h=87&zc=1&q=100 "Exception List Administration Panel")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/exception_list_administration.png "Exception List Administration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

9. A list of your installed modules will be displayed. Simply click “Add to Exception List” next to the module you want to exclude from “Block All” requests
10. To remove a module from the Exception List, click on “Remove from Exception List”

 

#### Insert Code Into Email Templates

Insert the following code snippet into the footer of the email templates for the modules you assigned to the Exempt List, replacing the opt-out code that already exists in the template footer:

**{if $noblock}**  
 This is an attempt to collect a debt. You cannot unsubscribe.  
**{else}**  
 <a href=”{$block\_url}”>Unsubscribe from this type of email</a>  
 |  
 <a href=”{$block\_all\_url}”>Unsubscribe from ALL emails</a>  
**{/if}**

   
 This will have the effect of displaying an “unsubscribe forbidden” notice, as well as making the links inactive so they cannot be clicked. If the module is ever removed from the Exempt List, then normal global and per-module unsubscribe links will be displayed.

Of course, you can edit the language used for the “unsubscribe forbidden” notice, as well as for the links themselves, by simply editing the above code snippet.

It is recommended to edit the link text in such a way as to make it clear to the customer what they are opting out of. For example, you might want to change

Unsubscribe from this type of email

to

Stop sending me \*\*\* emails

replacing the \*\*\* with the module name (i.e. Stop sending me **Birthday Greeting** emails, Stop sending me **Review Reminder** emails, etc). This will make it clear to the customer that they are only opting out of that specific type of email.

For global opt-outs, you may wish to change

Unsubscribe from ALL emails

to

Opt out of all non-administrative emails from \*\*\*\*

replacing the \*\*\*\* with your store’s name. This will make it clear to the customer that if they opt out of one, they opt out of all, but will continue to receive administrative emails such as purchase confirmations or password change confirmation emails.

### Block & Unblock Customers Globally or Per-Module

This feature is useful for unblocking customers who opted out accidentally or otherwise request to resume receiving emails again, block customers on a per-module basis, or blocking customers on a global basis.

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Configuration tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab2.png&w=270&h=175&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab2.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Opt-Out/Block Administration module and click on it.
5. Go to the Customer Block/Unblock Search and find the customer(s) you want to block or unblock by entering their first name, last name, full name, customer id, or email address:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/block_unblock_search.png&w=175&h=57&zc=1&q=100 "Block/Unblock Customer Search")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/block_unblock_search.png "Block/Unblock Customer Search")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**If you installed the Opt-Out dashboard widget, you can use it instead of the steps above to get to the Customer Block/Unblock Administration panel.**

8. The Customer Block/Unblock Administration panel is now visible:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_block_admin/block_unblock_config.png&w=270&h=126&zc=1&q=100 "Customer Block/Unblock Administration Panel")](http://www.mailbeez.com/images/doc/configbeez/config_block_admin/block_unblock_config.png "Customer Block/Unblock Administration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

10. If more than one customer is returned in the Search Results list, click the customer you wish to manage
11. To block individual email modules for this customer, simply click on “Block” next to the module(s) you wish to block
12. To unblock individual email modules for this customer, simply click on “remove” next to the module(s) you wish to remove the block for
13. To block the customer globally from receiving any MailBeez generated emails, click “Full Block”
14. To unblock the customer globally so they can resume receiving all MailBeez generated emails, click “Remove Full Block”
15. You can search additional customers if you need to by using the Search field at the top of the Customer Block/Unblock Administration Panel

 

### Allow Customers to Choose Their Opt-Outs

Making your opt-out links customer friendly and giving customers a choice of what to opt out of reduces your global opt-outs. There are three quick steps to making your opt-out links customer friendly:

- Set opt-out link behavior to “Module”
- Insert “Block All” links into your email templates
- Edit the link text to clarify for the customer what they are opting out of

#### Set Opt-Out Link Behavior to “Module”

First, make sure your Opt-Out Link Behavior setting in your Spam Compliance configuration settings are set to “Module”. If it is set to “Global”, then you already have “block all” links in your emails and customers won’t be able to choose which email modules to opt out of.

Ideally, you want two opt out links, one for global opt-outs and one for individual module opt-outs.

Navigate to: **admin > MailBeez > Configuration tab > Spam Compliance > Opt-Out Link Behavior**, set it to “Module” and click “Update”

 

#### Insert “Block All” Links Into Your Email Templates

Insert the following code snippet into the footer of the all your email templates (except for those on the Exempt List), replacing the opt-out code that already exists in the template footer:

<a href=”{$block\_url}”>Unsubscribe from this type of email</a>  
 |  
<a href=”{$block\_all\_url}”>Unsubscribe from ALL emails</a>

   
 This will have the effect of displaying both global and a per-module opt out links in the footers of every email template you insert this code into. This allows the customer to choose between blocking a specific type of email vs. blocking all MailBeez generated emails, thereby reducing your global opt-out rate!

 

#### Edit Opt-Out Links in Email Templates

It is recommended to edit the link text in such a way as to make it clear to the customer what they are opting out of. For example, you might want to change

Unsubscribe from this type of email

to

Stop sending me \*\*\* emails

replacing the \*\*\* with the module name (i.e. Stop sending me **Birthday Greeting** emails, Stop sending me **Review Reminder** emails, etc). This will make it clear to the customer that they are only opting out of that specific type of email.

For global opt-outs, you may wish to change

Unsubscribe from ALL emails

to

Opt out of all non-administrative emails from \*\*\*\*

replacing the \*\*\*\* with your store’s name. This will make it clear to the customer that if they opt out of one, they opt out of all, but will continue to receive administrative emails such as purchase confirmations or password change confirmation emails.



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.

## Template Manager

Mailbeez has developed a handy module that easily allows you to both edit and view your text changes right from the MailBeez interface within your store’s admin. Fully functional with all official MailBeez Modules (free, premium, and custom built), the MailBeez Template Manager makes editing a template a breeze, so much so that you may wonder how you ever lived without it! **[ Learn more!](/documentation/configbeez/config_tmplmngr/)**
