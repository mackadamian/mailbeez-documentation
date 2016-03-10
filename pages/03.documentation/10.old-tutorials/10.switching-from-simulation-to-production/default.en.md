---
# http://learn.getgrav.org/content/headers
title: Switching From Simulation to Production
slug: switching-from-simulation-to-production
# menu: Switching From Simulation to Production
date: 02-08-2012
published: true
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

 

## Take MailBeez Live

Once you have completed [testing](/documentation/tutorials/testing-mailbeez/), [email template customization](/documentation/tutorials/customizing-mailbeez-free-email-templates/), and [complete configuration](/documentation/tutorials/mailbeez-comprehensive-configuration-tutorial/) of your installation, you will be ready to switch from Simulation Mode to Production Mode and begin sending your first email campaign!

**Navigate to admin > MailBeez > Configuration tab > Simulation > Edit and set Mode to “production”:**

[![](http://www.mailbeez.com/images/doc/getting_started/set_mode.png "Mode Configuration Setting")](http://www.mailbeez.com/images/doc/getting_started/set_mode.png "Mode Configuration Setting")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

After saving your settings, you will see the status as “Mode: production”, indicating that the next time you run a MailBeez module it will send out real emails to your customers and track sending. To avoid duplication, once you have run a MailBeez module, it will not send new emails until there are “new” customers caught by the module’s query – which might be the next day or later depending on the module and size of your customer base.

To see copies of what MailBeez is sending out to your customers, you can configure the system to send you a copy of the emails. This feature is controlled by the “Send Copy”, “Send Copy To”, and “Max Number of Copy Emails Sent per MailBeez Module” configuration settings.. You should have configured these settings prior to testing, but now a change needs to be made.

**Navigate to admin > MailBeez > Configuration tab > Basic Configuration > Edit:**

[![](http://www.mailbeez.com/images/doc/getting_started/send_copy.png "Send Copy Configuration Setting")](http://www.mailbeez.com/images/doc/getting_started/send_copy.png "Send Copy Configuration Setting")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

“Send Copy” should be set to “yes”, but if it’s not, change that now. “Send Copy To” should already contain your email address, but if it doesn’t, change that now. Lastly, the configuration tutorial instructed you to set the “Max Number” setting to a high number for testing purposes. Now it is time to lower that number. Change this setting to something reasonable, like “10″.

Once you’re confident from reviewing the copies of emails being sent out that MailBeez is doing what it should do, you can return to this area and set “Send copy” to “False”.

 

## Using the Dashboard Mode Button

If you already know that your “Send Copy”, “Send Copy To”, and “Max Number of Copy Emails Sent per MailBeez Module” settings are as they should be, then a faster and simpler alternative is to use the “Mode” button on your MailBeez Dashboard.

Clicking this button not only changes the mode you’re in, but it also changes the button accordingly, so you know from a quick glance at your MailBeez Dashboard which mode you’re in:

[![](http://www.mailbeez.com/images/doc/getting_started/status_simulation.png "Dashboard Indicator Button: Simulation Mode")](http://www.mailbeez.com/images/doc/getting_started/status_simulation.png "Dashboard Indicator Button: Simulation Mode")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Note:**The “copy@localhost” that you see on the image above will be replaced by the email address you configure in the “Send Copy To” setting.

[![](http://www.mailbeez.com/images/doc/getting_started/status_production.png "Dashboard Indicator Button: Production Mode")](http://www.mailbeez.com/images/doc/getting_started/status_production.png "Dashboard Indicator Button: Production Mode")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)
