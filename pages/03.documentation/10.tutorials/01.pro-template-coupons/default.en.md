---
# http://learn.getgrav.org/content/headers
title: Creating template coupons
slug: creating-template-coupons
published: true
template: tutorial

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

>>>>>> use the tour within MailBeez to see how it works in your Store

In this tutorial you will learn how to create templates vouchers and configure the appropriate modules.


## Personalized Coupons

The MailBeez [Coupon Generator](/documentation/configbeez/config_coupon_engine) is used as a sub-module of all MailBeez modules generate and send that personalized coupons.

As an example for the module [coupon: Birthday Congratulations](/documentation/mailbeez/coupon_birthday) we go the steps to configure through - this procedure can be applied to all other MailBeez modules with coupon function.

## How it works

The MailBeez coupon generator generated based on a configured templates Coupons new vouchers. The generated certificate is a copy of the template voucher, but the  **expiration date** and **coupon code**  were generated individually. This ensures that every customer receives a personal coupon code that is only valid as long as the respective module (for example, "Voucher: Birthday congratulations") has been configured

## Creating a Template voucher

>>>>> Please ensure that the voucher system is activated (osCommerce: a [compatible coupon addon](/documentation/configbeez/config_coupon_engine) must be installed)

Navigate in the shop administration to the "vouchers".

Then click on "New voucher".

In the box **Coupon Code** (not name) enter the following: `template_birthday`.

It is important that the  **coupon code** starts with `template_` , as this identifies templates vouchers. Otherwise, the templates Voucher not be allocated in the following section.

Configure the templates voucher according to your wishes, for example, "10%" discount. Everything - except the expiration date - be transferred to the generated vouchers.

Save from the promo. (Important: after 1 click a page to verify the information is shown, then click again there speichner)

## Assigning the template coupon

Make sure that the newly created templates coupons can be seen in the coupon system of your shop.

then `MailBeez > MailBeez Modules Switch > Coupon: Birthday` and click there on the right side on top of the button **Edit** to open the Configuration view this module. Further down the right side you will find a selection list, from which you can select the created templates Voucher.

Save the configuration of the module.

In the view of the right you see at the bottom that the templates Voucher has been allocated.


## Find out more

### Testing the coupon generator

You can test using the "Simulation" the generation of coupons. Ensure cause MailBeez in the "Simulation" is (upper right corner) and run the module "Certificate: Birthday congratulations" from - there are "real" emails generated, but they are all configuration of the simulation sends e-mail address and marked with **[SIM]** in the subject.

In coupon system you will find for each email a generated coupon. The simulation coupons are marked with **[SIM]** in the coupon code. These coupons are fully functional, that is, You can hereby make test orders.

### Deleting Simulation vouchers

The scale in the simulation mode Vouchers can be deleted in the respective module with the structure appearing button. Alternatively you can use Generator the delete function in `MailBeez > Configuration > Certificate` .

### Deleting old Coupons
Over time, thousands of coupons will be generated. Under `MailBeez > Configuration > Coupon Engine` contains a handy "cleanup" function to delete lapsed coupons.


### Find vouchers

On the MailBeez Dashboard you can find a search function (eventually you need to install on `MailBeez > Configuration > Dashboard Configuration` ) that lets you quickly Coupons - find templates or vouchers and then to open it for editing.

>>>>>> Search for **template_** to find all template Vouchers and open directly to the editor