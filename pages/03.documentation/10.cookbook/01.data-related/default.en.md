---
# http://learn.getgrav.org/content/headers
title: data related
#menu: Beez-O-Graph
slug: data-related
date: 17-02-2016
published: true
publish_date: 17-02-2016
template: tutorial
# theme: false
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: done
    category: [docs]
    tag: [pro]
--------------

[TOC]


## check email-addresses of customer base

### Issue
In a 10 year old store very likely many email addresses have become invalid (email-addresses were deleted or do not accept more emails). Therefore it is necessary to check, which email-addresses are valid and to mark the invalid ones.


### Solution

We send out an info-email to all customers. Invalid email addresses will "bounce". This information is used to marked those email-addresses as invalid and to exclude them from future campaigns.

1. Subscribe to a MailBeez plan with [Newsletter Advanced](/documentation/mailbeez/newsletter)

1. In MailBeez configure the [Email-System](/documentation/configbeez/config_email_engine) to send through Newsletter2Go (if not done yet please register using the integrated form) and make sure you have enough volume (eventually charge your account)

1. Go to [Newsletter Advanced](/documentation/mailbeez/newsletter) and create a new list "all customer - no abo check". Configure in the segmentation of this list, for which countries the newsletter status should be ignored.

1. Go to [Newsletter Advanced](/documentation/mailbeez/newsletter) and create a new campaign using the list "all customer - no abo check". Within the campaign create a new email using following text (example - feel free to modify): 

 > To improve our customer service we want to make sure your Email-Address is still valid
 >  
 > In case you do not want to receive further information from us, please us the "no more emails" link in the footer of this email
 
1. activate the Newsletter and send it out.

Thanks to the integration of Newsletter2Go with MailBeez all invalid Email-addresses will be reported into MailBeez and excluded for future campaigns. This process can take a couple of days and can be monitored through the Beez-O-Graph > "bounces"
 

>>>>> When sending bulk emails invalid recipients increase the risk the sending email server gets rated as **sending out spam**. For this reason you should never use your own email-server, but use a **certified email system** like Newsletter2go.