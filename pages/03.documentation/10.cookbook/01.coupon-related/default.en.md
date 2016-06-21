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



## Coupon giveaway for registering to receive newsletters

>>>>>>  In compliance with certain exceptions, stores are allowed to contact their customers without explicit consent via email. Read more on [legal information](/about/legal-information)


### Requirement

You want to send your customers a coupon or voucher when they sign up for your newsletter

### Solution

Using the [Newsletter Advanced Module](/documentation/mailbeez/newsletter), you can customize and automatically send a store coupon to customers that register for the newsletter.

Just follow these steps:

####Create a dynamic list of recipients

1. Navigate to MailBeez Newsletter Module `MailBeez > MailBeez Modules > Newsletter Advanced`.
1. On the right hand side, click on button `Edit Lists`.
1. Create a new list, named e.g. `welcome coupon`. Select source `Shop Subscriber`. Click `insert` to save the list.
1. Select the newly created list and click on `edit segmentation` - a new window opens.
1. In segmentation settings, in section `customer`, configure the following:
    - Customer Signup Age Min: 0
    - Customer Signup Age Max: 1 (or a higher value if you want to send a coupon to past subscribers)
![List](Screen_welcome_list.en.png?lightbox=true)
1. Scroll down and click `update` to save the segmentation.
1. Back in the `Edit Lists` window, click `Test Segmentation` - you will now see customers matching the segmentation criteria - click on a customer, and the customer insight window opens.

You have now created a list of the latest newsletter subscribers.



####Create a Welcome newsletter

[plugin:content-inject](/content_blocks/pro_template_coupon_setup)


1. Navigate to MailBeez Newsletter Module `MailBeez > MailBeez Modules > Newsletter Advanced`. 
1. On the right hand side click on button  `Edit Campaigns`.
1. Create a new campaign named e.g. `Welcome newsletter`, and as default list, select the previously created list `welcome coupon` - click `insert` to save the campaign.
1. Select the newly created campaign and click on `Edit Campaign items`.
1. Create a new Newsletter - select the template - and click `New newsletter`.
1. Scroll down to `Select Coupon-Template for this Newsletter` to select or set-up a new coupon. Click `update` to save.
1. Configure the 'active until' date to 01/01/2099 (sets the newsletter to virtually never expire) and click `update` to save.
1. Now, design the email. Click on the + icon in the editor to add the layout element to display the coupon.
    - Note: If your store is set up for several languages, you need to design the other language templates as well.
1. Once you are happy with the design and test emails, you can click on `ready for sending` to activate the newsletter.    

![List](Screen_welcome_email.en.png?lightbox=true)

Congratulations! You have created a welcom newsletter, which will be send to the matching recipients the next time the sending process is triggered.
