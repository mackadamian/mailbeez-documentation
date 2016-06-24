---
# http://learn.getgrav.org/content/headers
title: Coupon Recipes
slug: coupon-recipes

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

Congratulations! You have now created a Welcome newsletter, which will be sent to all recipients matching your segmentation list the next time the sending process is triggered.





## Voucher as a product

### Issue
You want to allow your customers to purchase a voucher they can use as a gift


### Solution
Using the [Newsletter Advanced Module](/documentation/mailbeez/newsletter) you can automate a freely configurable voucher to your customers after purchasing one or more specific products. The voucher will be personalized. The voucher can be configured with all configuration options the coupon-system in your store offers - e.g. only 1 usage, limited to products/categories etc.


Please perform the following steps:
 
#### Create a product "gift voucher"
 
1. In your products catalog create a new category `Gift Voucher`
1. In this new category create a product e.g. `Gift Voucher 25 USD`
    - select a product description, product image etc.
    - set a price matching the value of the voucher

Now you have created a product, which represents the purchase of a voucher with 25 USD value. In the next step we will configure the Newsletter Advanced module to automatically send a voucher after the purchase of this product.


####Create a dynamic list of recipients

1. Navigate to MailBeez Newsletter Module `MailBeez > MailBeez Modules > Newsletter Advanced`
1. On the right hand site click on button `Edit Lists`
1. Create a new list, e.g. `gift voucher` with source `Shop Subscriber` - save the list.
1. Select the newly created list and click on `edit segmentation` - a new window opens
1. In the segmentation settings, section `geographical` configure the following:
    - Exclude following countries from newsletter check: enter all relevant countries so the voucher will be sent to every customer regardsless if they have subscribed for the newsletter or not
1. In the segmentation settings, section `products` configure the following:
    - pruchase products: `Gift Voucher 25 USD`
1. save the segmentation
1. with click on `Test Segmentation` you will see the matching customers - with click the customer insight opens

You have created a list which finds all customer who have purchase the product representing the gift voucher.





####Create the voucher email

[plugin:content-inject](/content_blocks/pro_template_coupon_setup)

1. Navigate to MailBeez Newsletter Module `MailBeez > MailBeez Modules > Newsletter Advanced` 
1. On the right hand site click on button  `Edit Campaigns`
1. Create a new campaign e.g. `Gift voucher Emails` and as default list select the previously created list `gift voucher` - save the campaign
1. Select the newly created campaign and click on `Edit Campaign items`.
1. Create a new Newsletter
1. On the right hand site select the template coupon - and save
1. Configure the active until date to e.g. 01/01/2099 (set the newsletter virtually to never expire) and save
1. Design the email, with click on the + icon in the editor you can add the layout element to display the coupon
    - In case your store is set up in several language please design the other language versions as well
1. Once you are happy with the design and test emails you can click on `ready for sending` to activate the newsletter 


Congratulations! You have created an email, which will be send to the customers who have purchase the gift voucher the next time the sending process is triggered.

If you would like to offer multiple gift vouchers, please repeat the steps for each.


>>>>> **Current limitation**:   
>>>>> for each customer and pruchase only 1 voucher can be sent  
>>>>> the expiry period is the globally configured period  
>>>>> **Please contact us in case you have additional requirements.**  
