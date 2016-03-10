---
# http://learn.getgrav.org/content/headers
title: BounceHive Bounce Handling
slug: bouncehive-bounce-handling-configuration-tutorial
# menu: BounceHive Bounce Handling
date: 07-08-2012
published: true
publish_date: 07-08-2012
# unpublish_date: 07-08-2012
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

## About This Module

Bounce emails that are not properly handled might result in an increased spam rating, so it is important to handle the inevitable email bounces that will come your way. The fully integrated BounceHive Bounce Handling from MailBeez allows you to automatically handle hard bounces, soft bounces and transient bounces.

## Requirements

- MailBeez V2.6
- A separate email account set up specifically for bounce handling & configured as an IMAP mailbox in your email client (more info below)
- Use of MailBeez own built in Email Engine – PHPMailer
- Your server must allow you to connect to IMAP servers – Check with your hosting company, especially if you plan to use GMail, as some have blocked the GMail-specific port

## Getting Started

### Set Up an Email Account Designated for Bounce Handling

It is strongly recommended that you set up an email account that is **only used to process bounce handling messages.** It should not to be used for sending or receiving any other type of emails.

This is because the Bouncehive module will process ALL mails in the inbox (top folder) of this account and move them to sub-folders which you will define in the Bounce Handler configuration settings. If you use this mailbox for sending and receiving other emails, you will get confused as mails are moved around between these sub folders by the module.

- Create the new account using your hosting company’s email service or some other mail service provider.

**If you are going to use Gmail, check with your hosting company for limitations as some have blocked the Gmail-specific port. If your hosting company has blocked the Gmail specific port, then you will need to use a mail service provider other than Gmail, or use your hosting company’s email service.**

- Make the email address something you will easily recognize as your bounce handling email account, perhaps “bounce@yoursite.com” for example.
- If you are using Gmail, you will need to go into your Gmail account settings and enable IMAP.
- Once the new account is created, you may need to configure the IMAP mailbox in an email client (such as Outlook) if your hosting company or other email service provider doesn’t provide IMAP mailbox functionality. Check with your hosting company or other email service provider to find out if this is the case for you.
- Test the new account by sending an email to and from it.

### Configure the PHP Mailer

1. Navigate to admin > MailBeez interface > Configuration tab > Email Engine
2. Click the “Edit” button to access the PHPMailer configuration settings

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/phpmailer_config.png&w=175&h=659&zc=1&q=100 "PHPMailer Configuration Settings")](http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/phpmailer_config.png "PHPMailer Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Configure the MailBeez PHPMailer settings using a separate email account **designated for bounce mail handling only.**
2. The settings below are mostly self explanatory, but for your convenience, a brief description of each has been provided.
3. The information you need to enter for the settings below will be provided to you by your hosting company or mail provider when you set up an SMTP (outgoing) mail account.
4. If you are using a Gmail account as your designated bounce handling email, see the “Using a Gmail Account for Bounce Handling” section below for additional information

**Select the Email Engine**  
 Select the PHPMailer option to switch from your store’s email system to the internal MailBeez PHPMailer system.

**PHPMailer: SMTP Username**  
 Enter the username for the email account you set up especially for bounce handling.

**PHPMailer: SMTP Password**  
 Enter the password for the email account you set up especially for bounce handling.

**PHPMailer: SMTP Server**  
 Enter the outgoing mailserver for the email account you set up especially for bounce handling.

**PHPMailer: SMTP Backup Server**  
 If available, enter the backup outgoing mailserver. If no backup server is available, leave this field blank.

**PHPMailer: SMTP Authentication**  
 Does your hosting company or other mail service provider require authentication of outgoing email?

**PHPMailer: SMTP Security**  
 Select what kind of security is required for the outgoing mailserver. By default, it is set to “None”. Check with your hosting company or other mail service provider to determine which setting is best for you.

**PHPMailer: SMTP Port**  
 Enter the port number required by your hosting company or other mail service provider for the outgoing mailserver. By default, it is set to port 25. You only need to change this if your hosting company or other mail service provider uses a different port for outgoing mail.

Typically, hosting companies and other mail service providers who would normally use port 25 will require a different port if you enable SSL or TLS security protocol and will advise you as to which port to use if enabling SSL or TLS.

**PHPMailer: TXT Format Only**  
 This setting lets you decide whether or not to send emails in txt format only. By default, it is set to “False”, meaning that emails may be sent in both html and txt format. Change it to “True” only if you want to send emails in txt format only.

**PHPMailer 5.2.1 DKIM Selector, Identity, Passphrase, Domain & Private**  
 DKIM is an acronym for DomainKeys Identified Mail, which is a method for associating a domain name to an email message, thereby allowing a person, role, or organization to claim some responsibility for the message. The association is set up by means of a digital signature which can be validated by recipients.

These settings are optional and required only for those opting to set up DKIM security. The information to be entered for these settings is available from your hosting company or other mail service provider if they offer the use of Domain Keys.

#### Using a Gmail Account for Bounce Handling

Setting up a Gmail account can be tricky. Here are some tips & required settings:

- Check with your hosting company for limitations as some have blocked the GMail-specific port. If your hosting company has blocked the GMail specific port, then you will need to use a mail service provider other than GMail, or use your hosting company’s email service.
- Enable IMAP in the Gmail account you’ve designated for use as your bounce mail handling account
- SMTP Server – enter imap.gmail.com
- SMTP Port – change from 25 to 993
- SMTP Security: Select the SSL option – **If you test in a local environment, your local environment must support SSL!**

### Install the Module’s Configuration Settings Into Your Database

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Configuration tab

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab2.png&w=270&h=175&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab2.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Locate the Bounce Handling module with the green plus sign (+) in front of it, and click on it.
2. Click on the Install button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/install.png&w=175&h=78&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/bouncehive_config.png&w=149&h=640&zc=1&q=100 "Bounce Handling Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/bouncehive_config.png "Bounce Handling Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

## Configuring the Module

### Unlock the Module

There are 3 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on either the second “Edit” button beneath “Certificate – Please Enter” or on the third “Edit” button at the bottom of the configuration panel (they both work)
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button
3. A valid certificate message will appear at the bottom of the configuration panel

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/valid_certificate_msg.png&w=175&h=55&zc=1&q=100 "Valid Certificate Confirmation Message")](http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/valid_certificate_msg.png "Valid Certificate Confirmation Message")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Your module is now unlocked and ready for configuration.

### Configure General Settings

Click the top-most “Edit” button to access the general settings:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/general_settings.png&w=111&h=640&zc=1&q=100 "Bounce Handling General Settings")](http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/general_settings.png "Bounce Handling General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “True” by default, meaning the module is on and ready to work. Change this setting to “False” to deactivate the module and disable it from being run.

**Process Bounce-Handling Automatically When MailHive is Run**  
 This settling lets you choose whether or not you want to process the bounce handling service each time an email module is run. It is set to “True” by default, but if you opt to set up a dedicated cron-job in order to control when the service is run, then you will want to change this setting to “False”.

For your convenience, the process URL that you need the dedicated cron-job to call is displayed beneath this setting. A dedicated cron-job would be useful if you have a slow email server resulting in PHP timeouts, or if you are running a lot of email modules and don’t need this service to run every single time every single module is run.

**BounceHive IMAP MailServer**  
 Enter the incoming MailServer for the email account you set up especially for bounce handling.

**BounceHive MailServer User Name**  
 Enter the username for the email account you set up especially for bounce handling

**BounceHive MailServer Password**  
 Enter the password for the email account you set up especially for bounce handling

**BounceHive MailServer Port**  
 By default, this setting is set to port 143. Leave this setting as it is unless you plan to use a different port for your incoming mail or are instructed to use a different port for your incoming mail by your hosting company or other mail service provider.

**BounceHive MailServer Security Option**  
 Select what kind of security is required for incoming mail. By default, this setting is set to “notls”. Check with your hosting company or other email service provider to find out if this setting is appropriate for you.

**BounceHive Max Messages**  
 This setting lets you define the maximum number of messages you want processed with every run of this module. By default, it is set to “500″, which should be a sufficiently high enough number to process all of your bounces in a single run. Hopefully you don’t have anywhere near that many bounces!

**PHPMailer: Sender Address (Return-Path)**  
 Enter the email address you set up especially for bounce handling. **Do not** enter the “Sender Address” email address you entered in your other individual email modules.

**The wording “Sender Address” is used throughout MailBeez as a synonym for “From Address” because for humans, they are the same thing. For mailservers, “Sender Address” is a return-path email address used for undeliverable mail, whereas “From Address” is a reply-to email address for delivered mail.**

When an email bounces, the mailsender will return it to the inbox of the email address you enter here, which **must be the email address you set up especially for bounce handling!** This email address is internal and is not visible to your customers, but is read by mailservers to determine where to send the bounce mail.

**Folder for Hard Bounced**  
 When this module is run for the first time, email folders are created in the inbox of the email account you set up especially for bounce handling. Either leave the default folder name in place or enter the name you prefer for the folder that will collect the hard bounce emails.

**Folder for Soft Bounced**  
 When this module is run for the first time, email folders are created in the inbox of the email account you set up especially for bounce handling. Either leave the default folder name in place or enter the name you prefer for the folder that will collect the soft bounce emails.

**Folder for Processed Emails**  
 When this module is run for the first time, email folders are created in the inbox of the email account you set up especially for bounce handling. Either leave the default folder name in place or enter the name you prefer for the folder that will collect the processed emails (emails that did not bounce).

**GMail will not auto-create folders. If you’re using a GMail account for your bounce handling, you will need to create 3 folders in your inbox which match the entries for the above 3 settings!**

**Softbounce: Delay**  
 This setting lets you tell MailBeez how many days to wait after an email soft bounces before the email is re-sent. After the configured number of soft bounces, the email will be converted into a hard bounce (see next setting). By default, it is set to “5″ meaning that MailBeez will wait 5 days after an email soft bounces before re-sending the email.

**Softbounce: Convert Into Hard Bounce Count**  
 This setting lets you tell MailBeez how many times an email can soft bounce before it is moved to the hard bounce folder and treated as a hard bounce. By default, it is set to “5″.

**Time Frame For Converting Soft Bounces Into Hard Bounces**  
 If an email soft bounces the configured number of times (see above setting) within this many days, it will be converted into a hard bounce. The default settings of 60 days and 5 soft bounces tells MailBeez, “if an email soft bounces 5 times within 60 days, convert it to a hard bounce”.

**Log Bounce Messages**  
 This setting lets you decide if you want bounce messages to be logged in your database. By default it is set to “True”, meaning that bounce messages will be logged in your database. Each bounce message can fill more than 1KB per bounce, so periodically you will want to manually empty this table. The bounce messages can be found in the table “mailbeez\_bounces\_msg\_log” in your database.

**PHPMailer: Override Sender Name and Address**

**This setting refers to the “Sender Name” and “Sender Address” settings in the individual email modules. *It does not refer to the “PHPMailer: Sender Address (Return-Path)” setting for this module*.**

Select “True” to override the “Sender Name” and “Sender Email” settings of the individual modules and instead use the “From Address” and “From Name” configured in the next two settings. If you leave it set to “False”, you will need to replace each module’s “Sender Address” with the email address you set up especially for bounce handling.

**How It Works**  
 Every MailBeez email module has a “Sender Address” setting which you configure after installing the module. The sender address is displayed in the emails generated by MailBeez and customers can see them and reply to the sender address.

In the modules, the wording “Sender Address” is a synonym for “From Address” because for humans, they are the same thing: the email address which sent the mail, is displayed in the email, and can be replied to.

Mailservers distinguish between “Sender Address” and “From Address”. “Sender Address” is a return-path email address used for undeliverable (bounced) mail, whereas “From Address” is a reply-to email address for delivered mail. This distinction is necessary for bounce handling so that the email address you set up for bounce handling will never be displayed to and used by customers.

This setting allows you to override the “Sender Name” and “Sender Address” in the individual modules and replace it with a global “From Name” and “From Address” which will display in emails to customers and provide them with an email address to which they may reply.

At the same time, the internal bounce handling email address, configured in the “PHPMailer: Sender Address (Return-Path)” setting for this module and invisible to customers, will be used by mailservers to return bounced mail.

**PHPMailer: From Address**  
 If you selected “True” for the “Override Sender Name and Address” setting, you will need to make an entry here. Keeping in mind that customers can see this in their emails, what email address do you want to appear as the “From Address” in outgoing emails? Customer replies will go to this email address.

**PHPMailer: From Name**  
 If you selected “True” for the “Override Sender Name and Address” setting, you will need to make an entry here. Keeping in mind that customers can see this in their emails, what name do you want to appear as the “From Name” in outgoing emails?

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!

## How Do I Use the Module?

It’s so easy! Begin by running a test to check the module’s connectivity to your mail server. To test, simply press the “Test” button on the module’s configuration panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/function_buttons.png&w=175&h=86&zc=1&q=100 "Bounce Handling Test & Run Buttons")](http://www.mailbeez.com/images/doc/configbeez/config_bouncehive_advanced/function_buttons.png "Bounce Handling Test & Run Buttons")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

When testing is complete, you can run the bounce handling manually by clicking either the “Run” button on the module’s configuration panel (see image above), or by going to admin > MailBeez > MailBeez Modules tab > Service Handler for Bounce Processing and clicking the “Run” button found there. Both “Run” buttons do the same thing, so which one you click on is purely a matter of personal preference.

Additionally, the bounce handling will be processed with every run of MailHive unless configured differently. In other words, unless you set “Process Bounce-Handling Automatically” to “False” in the module’s configuration panel, this module will run automatically every time an email module is run.

**This may cause PHP timeouts with slow email accounts. An alternative to the above is to deactivate the automatic run and set up a dedicated cronjob for running the bounce handling. The specific cronjob URL can be found in the module’s configuration panel.**

If you have saved historic bounce emails prior to the installation of this module, you should move those into the Bounce Handling email account you entered in the configuration panel. They will be automatically processed with the next run.
