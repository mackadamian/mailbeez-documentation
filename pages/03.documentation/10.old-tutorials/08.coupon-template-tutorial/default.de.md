---
# http://learn.getgrav.org/content/headers
title: Gutschein Vorlagen Tutorial
slug: gutschein-vorlage-tutorial
# menu: Gutschein Vorlagen Tutorial
date: 10-09-2012
published: true
publish_date: 10-09-2012
# unpublish_date: 10-09-2012
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

Übersetzung folgt

## About This Tutorial

The goal of this tutorial is to help you learn all about MailBeez coupons, from how they work to how you use them and everything in between. With that in mind, we will cover the following topics:

- About MailBeez Coupons & Coupon Templates
- Coupon Templates for Single Coupon Modules
- Coupon Templates for Multiple Coupon Modules
- Coupon Templates for the ReferralHoney Module
- Coupons in Simulation Runs vs. Test Emails
- Deleting Simulation Coupons
- What Can MailBeez Coupon Modules Do For You?

 

## About MailBeez Coupons & Coupon Templates

One of the nice things about using MailBeez for your coupon campaigns is that you don’t have to set up a thousand individual coupons, each with it’s own coupon code.

All you need to do is create one coupon template per email cycle per module, and MailBeez will use these master templates to create as many coupons with unique coupon codes as necessary to fulfill the demands of your modules when they are run. Very cool!

### Single Coupon Modules vs. Multiple Coupon Modules

Some modules, like the Birthday Greetings Coupon module, have only one email cycle and therefore require only one coupon template for that module. Other modules, like Winback Advanced, offer multi-step emailing and therefore require a coupon template for each email cycle.

The exception to this rule is the Send Coupon Campaign module. Although it has only one email cycle, it offers the ability to send as many coupon campaigns as you wish, with each campaign requiring its own coupon template. You cannot reuse an existing coupon template by just modifying it because the system tracks coupons sent & used based on the coupon id.

Since all of your customers will have already received a coupon with this coupon ID in the previous campaign, editing an existing coupon template for use in a new campaign would result in the email being sent out only to those customers which are new since the last run of the module.

### Viral Isn’t Always Desirable

A personalized coupon gives you total control over your store’s discount and coupon policy. To illustrate this, imagine if instead of using personalized coupons, you were to use the same coupon for every user.

In this instance, the risk of an unwanted viral effect is enormous. Just think what would happen if that code was pasted on a forum, or shared between friends? In one fell swoop you have lost control of your store’s coupon policy.

If you cancel the coupon in an attempt to regain control, loyal customers would be penalized and would not be able to take advantage of their discount. In an age of social marketing, the last thing you want to do is alienate your customer base.

### Safe With Mailbeez

With the personalized coupon creation ability of the Mailbeez premium modules, you not only protect your store’s discount policy, but also provide a more professional image whilst maximizing profit margins through intelligent coupon creation.

 

## Single Coupon Modules

As stated above, some modules have only one email cycle and therefore require only one coupon template for that module. Let’s use the ever popular Birthday Greeting Coupon module as our example of how to create coupon templates for single coupon modules.

### Creating the Coupons

1. Navigate to your store’s coupon administration area, either by using the “Set Up a Coupon Template” link in the module’s configuration panel, or by following the usual navigation path based on your e-commerce installation.
 

**The “Set Up a Coupon Template” link will disappear from a module’s configuration panel once coupon templates have been created for that module.**

4. Launch a new coupon
5. Configure the coupon settings:

**Coupon Name**  
 Coupon names are displayed in the coupon detail area of coupon emails, meaning that customers are able to see them. Choose a coupon name that will help you remember the purpose of the coupon, but will also be pleasing to customers. In this example, we will name the coupon “Birthday Coupon”.

**Coupon Description**  
 Leave this setting blank.

**Coupon Amount**  
 Enter the value of the discount for the coupon, either a fixed amount like 10.00, or a percentage like 10%

**Coupon Minimum Order**  
 If you want the customer to have to make a minimum purchase in order for the coupon to be valid, enter that amount here as a fixed amount like 25.00. Otherwise, leave it blank.

**Free Shipping**  
 Due to a limitation of the coupon systems included in most e-commerce platforms, you cannot offer both free shipping and a discount. If you wish to make the coupon valid for free shipping, check this box and remove the entry from the Coupon Amount field. Otherwise, leave this box unchecked.

**Coupon Code**  
 As stated earlier in this tutorial, MailBeez generates its own unique coupon codes. What you’re doing with this setting is creating the coupon template that MailBeez can use to generate those codes.

Therefore, all coupon codes must follow the naming convention of “*template*\_” followed by your desired coupon name in order to be usable by MailBeez. Additionally, only coupon templates beginning with “*template*\_” will be available in the drop-down menu in the module’s configuration panel.

For this module, let’s make the coupon code template\_birthday

**Uses per Coupon**  
 Remembering that MailBeez generates a unique coupon code for each customer it sends this coupon to, the easiest way to determine the best choice for this setting is to ask yourself “How many people do I want to be able to use each customer’s unique coupon code?”

You may set this to whatever you like, but the recommended setting is 1 unless you want multiple people to be able to use it. A setting of “1″ ensures that once the coupon is used, it cannot be used again by anyone, so if customers share it, it’s no big deal.

**Do not leave this setting blank unless you want the coupon to be used by an unlimited number of people for the duration of it’s validity period.**

Examples of the appropriate use of ‘unlimited coupon use’ would be the Share Coupon of the ReferralHoney module, or a timed coupon campaign from the Send Coupon Campaign module.

**Uses per Customer**  
 Remembering that MailBeez generates a unique coupon code for each customer it sends this coupon to, the easiest way to determine the best choice for this setting is to ask yourself “How many times do I want the customer to be able to use his coupon code?”

You may set this to whatever you like, but the recommended setting is 1 unless you want your customer to be able to reuse the coupon for some reason. A setting of “1″ ensures that once the customer uses the coupon, they may not use it again.

**Do not leave this setting blank unless you want the coupon to be available for unlimited use by the customer for the duration of it’s validity period.**

**Start Date & End Date**  
 Leave these settings blank. If your e-commerce platform provides a dropdown menu with pre-selected default dates, simply ignore the current settings. MailBeez will use the “Days Coupon is Valid” setting in the module’s configuration panel along with the date the module is run to calculate a coupon’s effective dates.

**Coupon Zone Restriction**  
 If you wish to restrict which zones a coupon is valid for, select from the dropdown menu. Otherwise, leave this setting blank.

When you’re done configuring your coupon, save it. You should see the new coupon template on your coupon list in the coupon administration area.

### Assigning the Coupon Template to the Email Module

1. Navigate back to the Birthday Greetings Coupon module in the MailBeez Modules tab.
2. Click the module’s “Edit” button to open its configuration panel.
3. Select “Birthday Coupon (template\_birthday)” from the Coupon Template dropdown menu & click the “Update” button.

Once you’ve completed creating, configuring, and assigning your coupon template, it’s time to send test emails and run simulations. But before you rush back to your module to do so, please check out the “Coupons in Simulation Runs vs. Testing” section of this tutorial if you are new to using coupons.

 

## Multi-Coupon Modules

The process for creating coupon templates is the same for multi-coupon modules as it is for single coupon modules, except for a few extra steps. With that in mind and using the Winback Advanced module as an example, follow the process as it is outlined above, except with the modifications shown below.

### Coupon Name & Coupon Code Settings

Multi-cycle coupon email modules require multiple coupons – one for each email cycle. In the case of Winback Advanced, there are 4 email cycles, so you will need to create 4 coupons.

Each coupon needs a coupon name and a coupon code. Remembering that **coupon names are displayed in emails to customers**, the below example is just that – an example, of how to create coupon names and coupon codes for multi-coupon modules.

You probably don’t want your customers to see a coupon named “Winback”, nor do you want them to see numbers after the coupon names, as this clues them in that more might be coming and could cause them to hold out.

You will want to create unique coupon names that are appropriate for customers and that make sense to you in terms of which module they work with.

 **Coupon Name** **Coupon Code**  Winback1 template\_winback1  Winback2 template\_winback2  Winback3 template\_winback3  Winback\_Loop template\_winback\_loop ### Assigning the Coupon Templates to the Module’s Email Cycles

Again, the process is the same here as it is for single coupon modules, except there are a few more steps:

1. Once you have configured and saved your final coupon, navigate back to the Winback Advanced Module > First Winback Email and click the “Edit” button to open its configuration panel.
2. Select “Winback1 (template\_winback1)” from the Coupon Template dropdown menu & click the “Update” button.
3. Navigate to the Second Winback Email and click the “Edit” button to open its configuration panel.
4. Select “Winback2 (template\_winback2)” from the Coupon Template dropdown menu & click the “Update” button.
5. Navigate to the Third Winback Email and click the “Edit” button to open its configuration panel.
6. Select “Winback3 (template\_winback3)” from the Coupon Template dropdown menu & click the “Update” button.
7. Navigate to the Winback Email Loop and click the “Edit” button to open its configuration panel.
8. Select “Winback\_Loop (template\_winback\_loop)” from the Coupon Template dropdown menu & click the “Update” button.

Once you’ve completed creating, configuring, and assigning your coupon templates, it’s time to send test emails and run simulations. But before you rush back to your module to do so, please check out the “Coupons in Simulation Runs vs. Testing” section of this tutorial if you are new to using coupons.

 

## ReferralHoney Coupons

The process for creating coupon templates for the ReferralHoney module is exactly the same as it is for any other multi-coupon template, with the exception of two settings for the Share Coupon. This is due to the fact that the Share Coupon will be used multiple times.

With that in mind, follow the process as it is outlined above, except with these modifications to the Share Coupon settings:

**Uses per Coupon**  
 Remembering that MailBeez generates a unique coupon code for each customer it sends this coupon to, the easiest way to determine the best choice for this setting is to ask yourself “How many people do I want to be able to use each customer’s unique coupon code?”

In this case, you would want the customer to share the coupon with as many people as possible, so the recommendation is to leave it blank. On the other hand, if you want to limit the number of people the customer can share the coupon with in order to keep control, set it to a number you feel comfortable with, but try to keep it in the higher range, 50 for example, because the goal here is to generate as many new sales as possible.

Also keep in mind that the Share Coupon is automatically marked as used for the customer who will be sharing it, so that they can’t use it. Therefore, if you’re going to enter a limit in this setting, add one more to it. For example, if you want the customer to be able to share this with no more than 25 people, set this to 26. The customer doing the sharing will count as the first use, leaving the coupon available for 25 more uses.

**Uses per Customer**  
 Set this to 1. This will prevent the people this coupon was shared with from using it more than once. Along with the fact that the Share Coupon will expire, this protects your store from being overwhelmed with coupon sales.

The coupon settings for the *Reward Coupons* should be the usual 1, and 1, unless for some reason you want customers to be able to share them with others or use them more than once.

 

## Coupons in Simulation Runs vs. Testing

Once you get your coupons created and assigned to their corresponding email cycles within your MailBeez modules, you’ll want to test them by running simulations and sending test emails.

When you do, you’ll notice some differing results between simulated runs and test emails in terms of what the coupon codes look like in the resulting emails and in the coupon admin area of your e-commerce installation.

Below are two bullet point lists comparing & contrasting test emails vs. simulations so that you can quickly & easily see the differences between them.

### Test Emails

Test emails are generated when you press the “Send” button in the “Send Test Email” section of your module’s configuration panel.

- Test emails use made up test data. Their purpose is to ensure the module is functioning and to give you a general idea of the email’s layout & design.
- Test emails do not generate real coupon codes.
- In test emails, the words “Test Code” will display in place of a coupon code.
- In test emails, the boxes containing the required orders & reward results **are not** populated with the data from your configuration settings.
- Because test emails don’t generate real coupon codes, no new coupons will appear in your store’s coupon administration area.

### Simulation Runs

Simulation emails are generated when you click the “Run” button in the “Run This Module” section of your module’s configuration panel.

- Simulation emails use real client data and look exactly as they will when you run the module in production mode.
- Simulation emails generate real coupon codes so you can see what your customer will see.
- In simulation emails, an actual coupon code is displayed. The code is preceded by [SIM], indicating that the coupon code was generated in simulation mode. In production mode, only the coupon code itself is displayed.
- In simulation emails, the boxes containing the required orders & reward results **are** populated with the data from your configuration settings.
- Because simulation emails generate real simulated coupon codes, you will see new coupons appearing in your store’s coupon administration area. This is to give you an idea of what you should see display there once you start sending out coupons in production mode.
- The new coupon will display on your coupon list with the same coupon code from the simulation email, preceded by [SIM], as the coupon name. This is so you can easily differentiate between the simulated coupons and production mode coupons on the coupon list.

 

## Deleting Simulation Coupons

Deleting simulation coupons is so easy! But please don’t try and delete them from your store’s coupon administration area. This will result only in the coupons being moved from the “Active Coupons” area to the “Inactive Coupons” area of your store. Unless you want to save your simulation coupons for some reason, follow these simple steps instead:

### Delete All Simulation Coupons

Following this process will delete **all** simulation coupons from your coupon list and your database.

1. Navigate to the Configuration tab of the MailBeez interface
2. Locate & click on the Coupon Engine to bring up it’s configuration panel
3. Click the “Delete” button beneath “Delete Simulation Coupons”

### Delete Simulation Coupons For Individual Modules

Following this process will delete simulation coupons from your coupon list and your database on a per-module basis.

1. Once you have run a simulation for a coupon module, a new function button will be added to that module’s general settings configuration panel.
2. Navigate to the MailBeez Modules tab of the MailBeez interface
3. Click on the module you wish to delete simulation coupons from and bring up it’s configuration panel
4. Click the “Delete” button beneath “Delete Simulation Coupons”

That’s all there is to it!

 

## MailBeez Coupon Modules

Have you fallen in love with a MailBeez coupon module? You’re in luck because MailBeez offers a huge variety of coupon modules that do everything from tempt your customers, reward your customers, turn your customers into word-of-mouth-social-marketers, and bring them back if they’ve forgotten about you.

There’s even a module to remind your customers when their coupons are getting ready to expire! Better pricing for them, more sales for you!

Take a look at the list below to see everything MailBeez can help you do with coupons.

- [**Birthday Greetings Coupon -**](/documentation/mailbeez/coupon_birthday/) Build customer loyalty by remembering them on their special day with a personalized coupon!
- [**Coupon Expiry Reminder -**](/documentation/mailbeez/coupon_expire/) Increase conversion of coupon emails by reminding customers when their coupons are about to expire!
- [**MailBeez ReferralHoney -**](/documentation/mailbeez/coupon_referral_honey/) Harness the power of social marketing by inviting your customers to refer you to their friends & then reward them when their friends buy!
- [**Nopurchase Advanced -**](/documentation/mailbeez/nopurchase_advanced/) Draw in customers who have never made a purchase by offering them coupons they can’t say no to!
- [**Reorder Advanced with Coupons -**](/documentation/mailbeez/reorder_advanced/) Tempt your customers to become repeat customers by enticing them with coupons!
- [**Review Reward Coupon -**](/documentation/mailbeez/coupon_review/) Reward your customers for writing product reviews in your store!
- [**Send Coupon Campaign -**](/documentation/mailbeez/coupon_campaign/) Create & manage specific coupon campaigns – perfect for holiday, special occasion, or seasonal campaigns!
- [**Winback Advanced -**](/documentation/mailbeez/winback_advanced/) Don’t forget about those old, inactive customers – tempt them back to your store using a multi-step coupon campaign until they just can’t say no!



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.

## Template Manager

Mailbeez has developed a handy module that easily allows you to both edit and view your text changes right from the MailBeez interface within your store’s admin. Fully functional with all official MailBeez Modules (free, premium, and custom built), the MailBeez Template Manager makes editing a template a breeze, so much so that you may wonder how you ever lived without it! **[ Learn more!](/documentation/configbeez/config_tmplmngr/)**
