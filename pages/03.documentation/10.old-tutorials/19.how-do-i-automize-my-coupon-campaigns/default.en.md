---
# http://learn.getgrav.org/content/headers
title: How do I Automate my Coupon Campaigns?
slug: how-do-i-automize-my-coupon-campaigns
# menu: How do I Automate my Coupon Campaigns?
date: 09-11-2010
published: true
publish_date: 09-11-2010
# unpublish_date: 09-11-2010
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
    name: admin
metadata:
    author: admin
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

An e-commerce store includes powerful coupon functionality, but often, creating a coupon campaign in order to reward or entice customers is frustratingly hard to administer. Ideally, you would like to track which coupons are sent out and finally used, and to do this you would need an intelligent system which not only finds qualifying customers, but then automatically generates personalized coupons. Luckily, all this and more is possible with MailBeez.

> ![](http://www.mailbeez.com/wp-content/uploads/2010/09/notification_warning_big.png "notification_warning_big")  
> **Please note:** This Tutorial is designed for Shop-Owners running on Zen-Cart, CRE Loaded, xt:Commerce, xtc-modified, Gambio GX and osCMax. These carts have by default a common, powerful in-built coupon system. If you are running osCommerce you need to install the CCGV(trad) addon, you can download this addon from [addons.oscommerce.com](http://addons.oscommerce.com/info/4135). The Coupon System of DigiStore is not supported, but you might be able to install the CCGV(trad) addon as well.

When designing a Coupon Campaign, you need to take into consideration how to make them both efficient (not too wordy!) and enticing, so let’s take a look at a few key pointers based on different triggers (customer behaviour), that should not be overlooked.

## 1. The Importance of a Coupon Expiration Date

![](http://www.mailbeez.com/wp-content/uploads/2010/09/notification_done_big.png "notification_done_big")With an expiration date you create a sense of **urgency**, and it is of the utmost importance that you include one in your campaigns. However, if an expiration date is many months away, the consumer is very likely forget about it. The way to avoid this situation is to make sure you are using an expiration date of **less than thirty days**, and consquently the consumer is more likely to use the coupon.

The MailBeez Coupon Modules are designed for times like this, and easily enable you to generate coupon codes with dynamic expiration dates. For example, you could configure an email to be sent with an embedded coupon that it is valid only for 14 days after receipt.

## 2. The Importance of individual Coupons

![](http://www.mailbeez.com/wp-content/uploads/2010/09/notification_done_big.png "notification_done_big")

When handing out online coupon codes you must be prepared for (in this case at least), an **unwanted viral effect**. Coupon codes are often posted on popular forums, which means that your precious discount codes can easily arrive into the hands of non-qualifying customers. If you allow this to happen, you not only risk alienating existing customers, but the gradual erosion of your hard fought for profit margins.

In order to prevent this, the MailBeez Coupon Modules can generate individual coupon codes per customer, giving you the tools to control how often a coupon code can be used. Since the coupons sent out are also tracked, you will be able to identify where a new order is coming from, or you can even **remind customers when their coupon code is going to expire** - which will again create a sense of urgency.

With MailBeez Coupon Modules you **get full control over your coupon campaigns**, plus the ability to completely automate them, leaving you with more time to get on with running important areas of your business, and less time on e-commerce administration.

# Step 1: Choose your Coupon Campaigns

**With MailBeez you can fully automize your coupon campaigns, so as the first step, you need to plan what kind of coupons you would like to send out.**

The kind of coupons you send out and in which time-frame is highly dependent on the products you are selling and in which market. A good idea might be to check out your competition and see what works for them.

**Reorder Coupon**

Send your customers a coupon for their next / second order, e.g.

> “10% off for your next order within the next 2 weeks!”

This type of coupon is perfect for products where customers can by add ons, upgrades or related products. You can utilize the positive “buying” attitude of a customer who has just ordered, and reward them for their loyalty.

**Winback Coupon**

In today’s ultra-competitive online world, getting customers is hard, and keeping them is even harder. With the Mailbeez Winback module, you can send any aged customer a reactivation email with a custom coupon code. For example, you could set up a campaign to email all customers who haven’t ordered in the last 6 months, writing something like this in the body:

> “We are missing you! Order within the next 10 days and get a 10% discount.”

Again, this is all fully automated – just install and forget.

**Birthday Coupon**

Your customers Birthday is the perfect opportunity to contact them with a special offer:

> “Happy Birthday! We really appreciate your business, so please enjoy a 15% discount off oyur next purchase if you order within the next 3 days”

**Review Coupon**

Saying thank you for a review might even help you to collect more reviews…

> “We would like to thank you for your recent review with a coupon for free shipping”

Customers are more likely to buy when they read the positive recommendations of others, so reviews are really important. Hey, even negative reviews might work –  especially if the store owner responds to it in a caring manner like “we have changed x in the current shipped products”. So why not reward your customers for writing a review for you?

**Seasonal Coupon Campaigns**

Perfect for seasons greetings, or special yearly events where you would like to send out a coupon to all customers:

> “5% off for all early-bird Christmas orders before 10th of December”.

When you send coupons through the MailBeez module, you are in full control how often each coupon can be used, you know who received that coupon and you can remind customers about the expiry of their unused coupon. This Module is typically used manually.

**Coupon Expiry Reminder**

With the amount of emails arriving in the average inbox numbering in the hundreds every day, it is a good idea to remind your customers of the impending expiry date of their unused coupon codes. Since all coupons sent through MailBeez Coupon Modules are tracked, you are able to easily follow-up and remind your customers in a timely manner of their expiration. For example, you might write:

> “Hey Bob, We wanted to write to let you know that your coupon will expire in 3 days, so act now to make sure you don’t miss out on this great saving!”

# Step 2: Setting up the Coupons

In order to see a list of defined coupons within Mailbeez, you first have to go to your store’s coupon admin area and set up individual coupon templates for each campaign you would like to run. Just make sure to follow these steps when you create the coupon:

- **Coupon code field **- Use the naming convention, ‘template\_couponname’ in this entry field, not a coupon code, as Mailbeez will create the coupon codes automatically, and individually for each email you send.
- **Coupon name field** – Enter the name of the coupon for easy retrieval later, for example ‘Birthday’
- **Coupon dates** – Please ignore these fields, as Mailbeez will override these settings in configuring the expiration date for your campaign
- **Uses per coupon** – Set this to ’1′

# Step 3: Set up the MailBeez Modules

Once the coupon templates are set up, go back to the MailBeez Module area within your store’s admin and assign the prepared coupon templates to your Mailbeez campaign (s) by choosing them from the drop-down list to the right hand side.

Once the coupon template(s) are assigned to the correct campaigns, set MailBeez into “Simulation”-Mode and run the module. When you are happy with the results, put MailBeez back to Production mode.

**NOTE** – During simulation testing, individually generated coupons will be marked with [SIM] to make them easy to distinguish and delete from your coupon area after testing.

 
