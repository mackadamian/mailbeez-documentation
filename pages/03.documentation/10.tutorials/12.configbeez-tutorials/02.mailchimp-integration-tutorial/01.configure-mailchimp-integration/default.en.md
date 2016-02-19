---
# http://learn.getgrav.org/content/headers
title: Configure MailChimp Integration
slug: configure-mailchimp-integration
# menu: Configure MailChimp Integration
date: 01-11-2012
published: true
publish_date: 01-11-2012
# unpublish_date: 01-11-2012
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

## Set MailBeez to Simulation Mode

Begin the configuration process by putting MailBeez into Simulation mode:

1. Log in to your store’s admin interface & navigate to your MailBeez interface
1. Check to see if what mode you’re in. Production mode will have a green “Production” button in the upper right corner and Simulation mode will have an orange “Simulation” button in the upper right corner
1. If you’re in Production mode, click the green button to switch to Simulation mode. If you’re already in simulation mode, proceed to the next step

## Complete the Installation

1. Navigate to the Configuration tab
1. Locate the MailChimp Integration module and click on it.
1. Click on the Install button to install the configuration settings into your database
The configuration panel is now visible
 

## Using the Configuration Wizard

With the built in configuration wizard, configuring your module couldn’t be easier! Since the wizard saves your settings as you go, if you need to step away for any reason, you can always come back and complete the configuration by picking up where you left off. Handy!

Begin by clicking the “Start Wizard” button on the configuration panel and follow the steps by providing the information requested for each configuration setting:

1. Enter Your MailChimp API Key  
 Enter the MailChimp API key available from your MailChimp account. If you have not yet created an API Key for MailBeez, you will need to do that now. If you don’t know how, use the link in the wizard to a tutorial on the MailChimp website.
 
2. Select Your Integration Mode  
 Select the Integration mode that matches the List Management option you chose earlier – Option A, Option B, or Option C.
3. Assign the Test List(s) to the Integration Mode  
 In the “Getting Started” portion of the tutorial, you were guided to create test lists based on how you wish to manage your subscription lists. In this step, you will assign the list(s) you created to the Integration mode you selected in the previous step. 
 
 Select which email engine you’d like to use to send out your MailBeez generated emails & then click the “Save & Next” button.
 **Default**  
 MailBeez generated emails will be delivered by your store’s mail engine.  
 **MailChimp**  
 MailBeez generated emails will be delivered solely through MailChimp. Customers not subscribed to a MailChimp list will not receive an email.  
 **MailChimp with Fall Back**  
 MailBeez generated emails will be delivered through MailChimp for all users subscribed through MailChimp, and your store’s email engine if a user is not subscribed through MailChimp.

1. Assign MailChimp Templates

## Next Step

Now that you’ve completed the configuration, it’s time to do some testing! It is extremely important to conduct testing before taking the module live because once the module is live, newsletters and email campaigns will be sent to real customers and of course you want to prevent mistakes from ending up in your customer inboxes.

[Step 2: Test MailChimp Integration](/documentation/tutorials/configbeez-tutorials/mailchimp-integration-tutorial/test-mailchimp-integration/)
