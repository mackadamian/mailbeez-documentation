---
# http://learn.getgrav.org/content/headers
title: Testing MailBeez
slug: ID-4971
# menu: Testing MailBeez
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

## Testing MailBeez is Easy!

Once you’ve [configured](/documentation/tutorials/mailbeez-comprehensive-configuration-tutorial/) MailBeez, it’s time to test each of your MailBeez modules. MailBeez offers a very safe and intuitive testing system which allows you to test in 3 simple steps:

- View the email templates
- Send a test email to a preferred email address
- Run MailBeez Modules in Simulation mode

In order to test MailBeez, you must have at least one email module installed. Let’s use the Birthday Greetings module as an example.

## Install the Birthday Greetings Module


1. Navigate to admin > MailBeez Interface > MailBeez Modules tab > Birthday Greetings
2. Click on the “Install” button:

[![](http://www.mailbeez.com/images/doc/mailbeez/birthday/birthday_config2.png "Install Birthday Greetings")](http://www.mailbeez.com/images/doc/mailbeez/birthday/birthday_config2.png "Install Birthday Greetings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. This will bring up the Birthday Greetings module configuration panel.
2. Go to “Activate Module”, click “True”, & click “Update” to turn the module on.

The remaining configuration settings are fine for testing purposes. If you need help changing them later, please visit the [Birthday Greetings Configuration Tutorial](/documentation/tutorials/mailbeez-tutorials/birthday-greetings-configuration-tutorial/)

## Testing MailBeez

Visit your MailBeez email modules one at a time and test them as follows:

### View the Email Templates

The “HTML” and “TXT” buttons let you preview the static text and style of the email templates.

[![](http://www.mailbeez.com/images/doc/getting_started/preview_templates.png "Preview Templates")](http://www.mailbeez.com/images/doc/getting_started/preview_templates.png "Preview Templates")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Placeholder content like ‘{$firstname}’ for example, show you where the dynamic data will be inserted in the final email. This placeholder content does not display in the email when the module is run. Instead, it is replaced with the information it represents (such as the customer’s first name, for example), as you will see in the next step when you send a test email.

### Send a Test Email

This function allows you to send a quick test email to a preferred email address. It’s a great feature for checking layout, text and style changes in your email as you work on a template. Because it is a test email, it uses test data rather than real data, so don’t be concerned if the date is incorrect or the customer name is strange.

You will be able to see real customer data in your testing when you move on to the next step, “Run Your MailBeez Modules in Simulation Mode”. For now, let’s take a look at the “Send Test Email” button and how to best use it. The purpose of this step is to confirm that the customizations you made to your email templates are rendering as you expect.

[![](http://www.mailbeez.com/images/doc/getting_started/send_test.png "Send Test Email")](http://www.mailbeez.com/images/doc/getting_started/send_test.png "Send Test Email")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

When you click on the send button, you will get a popup screen in which you’ll be able to enter the email address where you want the test email to go to. It is a good idea to send a test email to an email address which is configured to receive email in HTML format, and send a second test email to an email address which is configured to receive email in TXT only format.

This way, you can see what your customers will see whether they are receiving mail in HTML or TXT format. This process ensures both your HTML and TXT format emails look sharp & professional. There is nothing more embarrassing than getting emails from customers saying your emails are poorly formatted or contain errors.

### Run Your MailBeez Modules in Simulation Mode

When you are happy with the appearance of your email templates, the next step is to run a simulation.

**What Does “Simulation Mode” Mean?**  
 In simulation mode, MailBeez will generate emails just like production mode, but will send the emails only to your configured “Send Copy To” email address. This email address can be [configured](/documentation/tutorials/mailbeez-quick-start-configuration-tutorial/) in the “MailHive – Basic Configuration” area.

[![](http://www.mailbeez.com/images/doc/getting_started/send_copy_to.png "Configure Send Copy To Email Address")](http://www.mailbeez.com/images/doc/getting_started/send_copy_to.png "Configure Send Copy To Email Address")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

When you run a simulation, you will see exactly what your customers will see, without actually sending them anything; smart, hey?

**Prepare Data for Running a Simulation**  
 To run a successful simulation you need to make sure you have customers matching the modules’ criteria. For example, for the “Winback” module, you would need to have a list of customers who have not ordered within the time frame you configured in your Winback module.

When you click the “Show Recipients” button, you will see a list of customers who would receive this email if you were in Production Mode, but since you are in Simulation Mode, the emails generated will be sent to your “Send Copy To” address instead of to your customers.

[![](http://www.mailbeez.com/images/doc/getting_started/view_recipients.png "View Recipients")](http://www.mailbeez.com/images/doc/getting_started/view_recipients.png "View Recipients")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Later, when you put MailBeez in “Production Mode”, it will be this same list of customers will receive the generated email.

**Running a Simulation:**  
 To run a simulation click on this button:

[![](http://www.mailbeez.com/images/doc/getting_started/run_module.png "Run Module")](http://www.mailbeez.com/images/doc/getting_started/run_module.png "Run Module")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

You’ll notice that this button respects the mode, meaning that when you’re in simulation mode, it will say “Run this module in mode: simulation”. When you’re in production mode, it will say “Run this module in mode: production”, as it does in the screen shot above.

This serves as a reminder of what mode you’re in so that you don’t accidentally email your customers when you thought you were running a simulation.

Once you click this button, a pop up will appear and ask for you to confirm the simulation.

**Clearing Simulation Data Between Simulation Runs**  
 Remember reading that MailBeez won’t send the same email to the same customer twice? Well, this is also true in Simulation Mode, so if you need to run a simulation more than once, you must clear your simulation data between simulated runs. This is very easy to do: simply click the orange Simulation Restart button in the top right corner of your MailBeez user interface:

[![](http://www.mailbeez.com/images/doc/getting_started/restart_simulation.png "Restart Simulation")](http://www.mailbeez.com/images/doc/getting_started/restart_simulation.png "Restart Simulation")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In other words, during testing it is not uncommon to follow this process as often as you need to:

- Click the “Run” button to run the simulation
- Click the “Simulation Restart” button to clear the simulation data from that run
- Click the “Run” button to run the simulation again

## Switching to Production Mode

When you’ve completed testing and are satisfied that all is as it should be, you’re ready to switch over to Production Mode and take MailBeez live! This is very easy to do, involving a quick review of a couple of settings and the changing of the mode setting. When you’re ready to switch over to Production Mode, take a look at the [Switching From Simulation to Production tutorial](/documentation/tutorials/switching-from-simulation-to-production/) which walks you through this quick & easy process.
