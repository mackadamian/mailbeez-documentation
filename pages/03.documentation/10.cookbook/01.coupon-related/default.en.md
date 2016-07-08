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
1. Back in the `Edit Lists` window, click `Test Segmentation` - you will now see customers matching the segmentation criteria - click on a customer, and the Customer Insight window opens.

You have now created a list of the latest newsletter subscribers.



####Create a Welcome newsletter

[plugin:content-inject](/content_blocks/pro_template_coupon_setup)


1. Navigate to MailBeez Newsletter Module `MailBeez > MailBeez Modules > Newsletter Advanced`. 
1. On the right hand side click on button  `Edit Campaigns`.
1. Create a new campaign named e.g. `Welcome newsletter`, and as default list, select the previously created list `welcome coupon` - click `insert` to save the campaign.
1. Select the newly created campaign and click on `Edit Campaign items`.
1. Create a new Newsletter - select the coupon template - and click `New newsletter`.
1. Scroll down to `Select Coupon-Template for this Newsletter` to select or set-up a new coupon. Click `update` to save.
1. Configure the 'active until' date to 01/01/2099 (sets the newsletter to virtually never expire) and click `update` to save.
1. Now, design the email. Click on the + icon in the editor to add the layout element to display the coupon.
    - Note: If your store is set up for several languages, you need to design the other language templates as well.
1. Once you are happy with the design and test emails, you can click on `ready for sending` to activate the newsletter.    

![List](Screen_welcome_email.en.png?lightbox=true)

Congratulations! You have now created a Welcome newsletter, which will be sent to all recipients matching your segmentation list the next time the sending process is triggered.





## Voucher as a gift product

### Requirement
You want to give your customers the option to purchase a store voucher that they can use as a gift.


### Solution
Using the [Newsletter Advanced Module](/documentation/mailbeez/newsletter) you can customize and automate a configurable voucher that customers can purchase as an individual product. The voucher can be configured with all configuration options available in your store coupon-system - e.g. one time use, limited to products/categories etc. The voucher is unique, but not personalized. 

Just follow these steps:
 
#### Create a "gift voucher" product
 
1. In your products catalog create a new category `Gift Voucher`
1. In this new category create a product named e.g. `Gift Voucher 25 USD` (use relevant currency)
    - Select a product description, product image etc.
    - Set a price matching the value of the voucher

Now you have created a new product, which is a voucher and represents the purchase of a voucher with a value of 25 USD. In the next step we will configure the Newsletter Advanced module to automatically send a voucher after the purchase of this product.


####Create a dynamic list of recipients

1. Navigate to MailBeez Newsletter Module `MailBeez > MailBeez Modules > Newsletter Advanced`.
1. On the right hand side, click on button `Edit Lists`.
1. Create a new list, name it e.g. `gift voucher`. Select source `Shop Subscriber`. Click `insert` to save the list.
1. Select the newly created list and click on `edit segmentation` - a new window opens.
1. In the segmentation settings, section `geographical` configure the following:
    - Exclude following countries from newsletter check: (you should enter all relevant countries so the voucher can be sent to a customer regardless if they have subscribed to the newsletter or not).
1. In the segmentation settings, in section `products`, configure the following:
    - Products purchased: Select a voucher product you created e.g. `Gift Voucher 25 USD`.
1. Click `update` to save the segmentation.
1. Click on `Test Segmentation`- you will now see customers matching the segmentation criteria - click on a customer, and the Customer Insight window opens.

You have now created a list which finds all customers who have purchased the product Gift Voucher.





####Create the voucher email

[plugin:content-inject](/content_blocks/pro_template_coupon_setup)

1. Navigate to MailBeez Newsletter Module `MailBeez > MailBeez Modules > Newsletter Advanced` 
1. On the right hand side click on button  `Edit Campaigns`
1. Create a new campaign named e.g. `Gift Voucher Emails`, and as default list, select the previously created list `gift voucher` - click `insert` to save the campaign.
1. Select the newly created campaign and click on `Edit Campaign items`.
1. Create a new Newsletter - select the coupon template - and click `New newsletter`.
1. Scroll down to `Select Coupon-Template for this Newsletter` to select or set-up a new coupon. Click `update` to save.
1. Configure the 'active until' date to 01/01/2099 (sets the newsletter to virtually never expire) and click `update` to save.
1. Now, design the email. Click on the + icon in the editor to add the layout element to display the coupon.
    - Note: If your store is set up for several languages, you need to design the other language templates as well.
1. Once you are happy with the design and test emails, you can click on `ready for sending` to activate the newsletter.


Congratulations! You have created an email, which will be sent to the customers who have purchase the gift voucher the next time the sending process is triggered.

To offer multiple gift vouchers, just repeat the steps above for each additional gift voucher.


>>>>> **Current limitations**:   
>>>>> Only 1 voucher can be sent for each customer, and for each purchase.  
>>>>> **Please contact us in case you have additional requirements.**  
