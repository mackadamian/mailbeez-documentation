---
# http://learn.getgrav.org/content/headers
title: Using the MailBeez Version Check Widget
slug: ID-5002
# menu: Using the MailBeez Version Check Widget
date: 02-08-2012
published: false
publish_date: 02-08-2012
# unpublish_date: 02-08-2012
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

 

## About This Tutorial

Keeping MailBeez up to date and functioning properly couldn’t get any easier! There are two options available for keeping the MailBeez framework and your modules up to date: the MailBeez Check for Updates email module, and the MailBeez Version Check widget.

This tutorial will focus on using the MailBeez Version Check widget on your MailBeez Dashboard. Alternatively, you may wish to use the [MailBeez Check for Updates email module](/documentation/tutorials/mailbeez-tutorials/mailbeez-check-for-updates-configuration-tutorial/)

 

## The MailBeez Version Check Widget

The MailBeez Dashboard includes a cool widget for checking your MailBeez framework and modules for updates. All you have to do is click on “Check for Update” and the software will automatically check itself to see if new versions are available. If updates are available, you will see the widget change to provide color-coded information: orange for updates and blue for newly released modules you may want to consider installing:

[![](http://www.mailbeez.com/images/doc/getting_started/version_check.png "Version Check Widget")](http://www.mailbeez.com/images/doc/getting_started/version_check.png "Version Check Widget")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Clicking the “Check for Updates” button will also result in seeing the same color-coded update indicators on the tabs which alert you to updates and new modules by category:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/getting_started/version_check_tabs.png&w=540&h=55&zc=1&q=100 "Update Indicators")](http://www.mailbeez.com/images/doc/getting_started/version_check_tabs.png "Update Indicators")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Clicking on any tab displaying update indicators will result in being taken into that tab where you’ll see a list of newly available modules and your familiar list of installed modules with indicators as to which modules are in need of updating:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/getting_started/new_mods.png&w=540&h=202&zc=1&q=100 "Newly Available Modules")](http://www.mailbeez.com/images/doc/getting_started/new_mods.png "Newly Available Modules")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/getting_started/update_mods.png&w=540&h=241&zc=1&q=100 "Module Update Buttons")](http://www.mailbeez.com/images/doc/getting_started/update_mods.png "Module Update Buttons")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Modules in need of an update will have an orange “New Version” button next to them. Clicking this button takes you directly to the updated module on the MailBeez website.

Now that you know how to use the Version Check widget to identify which modules need updating, let’s talk briefly about how to actually update the modules.

 

## How to Update MailBeez Modules

Each module comes with a step-by-step update.txt file that walks you through the process. You will see that updating MailBeez modules is quick and easy. Once you’ve used the Version Check widget to identify which of your modules need updating, follow these simple steps:

### Updating Free MailBeez Modules

- Click on the “New Version” button next to the module that needs updating to go to the module’s page on the MailBeez website
- Download the fileset & unzip it on your computer
- Using FTP, navigate to that mod’s template files and download your customized versions
- Replace the template files in the fileset with the customized versions you just downloaded
- Follow the step-by-step instructions in the upgrade.txt file included in the fileset so you’ll know which module files need replacing

### Updating Premium MailBeez Modules

- Download the updated fileset from Avangate using the download link from the delivery email. If you have lost this information, log in to your account at avangate.com and download from there.
- Unzip the downloaded fileset on your computer
- Using FTP, navigate to that mod’s template files and download your customized versions
- Replace the template files in the fileset with the customized versions you just downloaded
- Follow the step-by-step instructions in the upgrade.txt file included in the fileset so you’ll know which module files need replacing
