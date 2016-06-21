---
# http://learn.getgrav.org/content/headers
title: Coupon Recipes

routes:
    aliases:
        - /documentation/cookbook/newsletter-related

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

---

[TOC]



## Voucher for registering for newsletter

>>>>>>  In compliance of certain exemptions store owner are allowed to contact their customers without explicit consent via email, read more on [legal information](/about/legal-information)


### Issue

You want to send your customers a coupon when they sign up for the newsletter

### Solution

Using the [Newsletter Advanced Module](/documentation/mailbeez/newsletter) you can automate a freely configurable voucher to your customers by registering for the newsletter.

Please perform the following steps:

####Create a dynamic list of recipients

1. Navigate to MailBeez Newsletter Module `MailBeez > MailBeez Modules > Newsletter Advanced`
1. On the right hand site click on button `Edit Lists`
1. Create a new list, e.g. `welcome voucher` with source `Shop Subscriber` - save the list.
1. Select the newly created list and click on `edit segmentation` - a new window opens
1. In the segmentation settings, section `customer` configure the following:
    - Customer Signup Age Min: 0
    - Customer Signup Age Max: 1 (or a higher value if you want to sent a coupon to historic subscribers)
![List](Screen_welcome_list.en.png?lightbox=true)
1. save the segmentation
1. with click on `Test Segmentation` you will see the matching customers - with click the customer insight opens

You have created a list which finds the latest newsletter subscribers.



####Create a welcome newsletter

[plugin:content-inject](/content_blocks/pro_template_coupon_setup)


1. Navigate to MailBeez Newsletter Module `MailBeez > MailBeez Modules > Newsletter Advanced` 
1. On the right hand site click on button  `Edit Campaigns`
1. Create a new campaign e.g. `Welcome Emails` and as default list select the previously created list `welcome voucher` - save the campaign
1. Select the newly created campaign and click on `Edit Campaign items`.
1. Create a new Newsletter
1. On the right hand site select the template coupon - and save
1. Configure the active until date to e.g. 01/01/2099 (set the newsletter virtually to never expire) and save
1. Design the email, with click on the + icon in the editor you can add the layout element to display the coupon
    - In case your store is set up in several language please design the other language versions as well
1. Once you are happy with the design and test emails you can click on `ready for sending` to activate the newsletter    

![List](Screen_welcome_email.en.png?lightbox=true)

Congratulations! You have created a welcome newsletter, which will be send to the matching recipients the next time the sending process is triggered.


## Voucher as a product

todo
