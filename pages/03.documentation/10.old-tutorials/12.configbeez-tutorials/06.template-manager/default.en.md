---
# http://learn.getgrav.org/content/headers
title: Template Manager
slug: template-manager
# menu: Template Manager
date: 23-08-2012
published: true
publish_date: 23-08-2012
# unpublish_date: 23-08-2012
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

Say goodbye to downloading template files, editing & saving them on your local drive, uploading them back to your server, and viewing them online only to have to go back and repeat the process after every change.

Template Manager allows you to easily edit and view your text changes right from the MailBeez area within your store’s admin! It is fully functional with all official (free and premium) MailBeez Modules as well as with custom built modules, making template editing a breeze – so much so that you may wonder how you ever lived without it!

## Getting Started


1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Configuration tab

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab2.png&w=270&h=175&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab2.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Locate the Template Manager module and click on it.
2. Click on the “Install” button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_install.png&w=175&h=74&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_config_panel_locked.png&w=175&h=225&zc=1&q=100 "Template Manager Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_config_panel_locked.png "Template Manager Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

## Configuring the Template Manager Module

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on second “Edit” button at the bottom of the configuration panel
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready for configuration.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_config_panel_unlocked.png&w=175&h=280&zc=1&q=100 "Unlocked Template Manager Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_config_panel_unlocked.png "Unlocked Template Manager Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Configure General Settings

Click the first “Edit” button at the top of the configuration panel to access the general settings. There are 2 of them:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_general_settings.png&w=175&h=157&zc=1&q=100 "Template Manager General Settings")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_general_settings.png "Template Manager General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “True” by default, meaning the module is on and ready to work. Change this setting to “False” to deactivate the module and disable it from being used.

**Select Your Template Theme**  
 This setting lets you choose which template theme you want to use. By default, it is set to “Default”, meaning it will use the template theme that came pre-installed with your MailBeez software.

When you have completed your configurations, click the “Update button”. Configuration of the module is now complete!

## How Do I Use Template Manager?

The processes for using Template Manager to edit & customize your email templates are slightly different between MailBeez premium email templates and MailBeez free email templates because MailBeez premium email modules provide you with many more options than do MailBeez free email modules.

For example, MailBeez free email modules allow for a single theme (utilizing the Common Main templates) and a single layout style (utilizing each module’s body\_html.tpl file), whereas MailBeez premium email modules allow for multiple themes and layout styles, as well as the ability to create custom versions of each and switch between them as desired.

For this reason, we have separated these processes into two different sections within this tutorial for easier use & understanding.

## Using Template Manager With Premium Email Templates

**Before you begin using Template Manager to edit your premium email templates, you must create custom templates rather than making edits directly to the templates that came pre-installed with MailBeez and your Premium MailBeez modules to avoid losing your customizations when using Template Manager to switch between templates.**

This is because Template Manager is designed to protect the integrity of the original templates that come pre-installed with MailBeez and your Premium MailBeez modules. If a template gets broken during editing, this allows you to restore the originals and start over. This functionality also comes in to play when you switch between templates, so if you don’t have custom templates set up, edits you make to the original files will be lost.

**An overview of theme templates vs. layout style templates, as well as step-by-step instructions for creating custom templates & backing up your customizations can be found in the [Customizing MailBeez Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)**

### Editing Custom Theme Templates

Once you’ve created your custom theme templates using the Customizing MailBeez Premium Email Templates tutorial, it is safe to begin with your custom edits. Customizing theme templates can be done in just a few easy steps:

#### Select a Custom Theme to Edit

Using the custom theme you created, for example “**mydefault**“, navigate to ** admin > MailBeez > Configuration tab > Template Manager module:**

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_config_panel_unlocked.png&w=175&h=280&zc=1&q=100 "Unlocked Template Manager Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_config_panel_unlocked.png "Unlocked Template Manager Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Click on the “Edit” button at the top of the configuration panel to access your configuration options:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/theme_selector.png&w=175&h=107&zc=1&q=100 "Template Manager Configuration Setting - Theme Selector")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/theme_selector.png "Template Manager Configuration Setting - Theme Selector")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Select the new custom theme template you created, for example “**mydefault**“, and click the “Update” button.

#### Launch Template Manager’s Template Editor

Remembering from the Customizing MailBeez Premium Email Templates tutorial that Theme templates and Common Main templates are in fact one in the same, click on the Common Main Template “Edit” button on the Template Manager configuration panel to access the Common Main templates in the template editor:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor.png&w=270&h=128&zc=1&q=100 "Template Manager - Template Editor")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor.png "Template Manager - Template Editor")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

#### Load the New Custom Theme Templates

You’ll notice that the templates which are automatically loaded are the last templates you were editing (or the default templates if this is your first time using Template Manager). To load the new custom template files, you must click the “Restore” button. This has the dual function of both loading your custom templates, and also restoring the the previous templates to their original state.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/restore_button.png&w=175&h=262&zc=1&q=100 "Template Editor Restore Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/restore_button.png "Template Editor Restore Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

This is why it was so important to first make a set of custom templates before getting started because if you had made edits to the default templates, and then later came here to edit a new custom theme template, you would have lost all of the customizations you made to the default templates.

#### Edit the Custom Theme Templates

In the Template Manager’s template editor, you can edit both the HTML and TXT templates, preview how the changes appear in the templates, send a test email, or restore your templates back to their original content if you break something or just want to undo all of your changes.

In the HTML template editor, you can customize images, text, style, layout and content:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_html.png&w=270&h=106&zc=1&q=100 "Template Editor - Custom Theme HTML Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_html.png "Template Editor - Custom Theme HTML Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In the TXT template editor, you can customize text, add or remove template variables, and determine the order in which text & template variables will appear in the email:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_txt.png&w=175&h=120&zc=1&q=100 "Template Editor - Custom Theme TXT Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_txt.png "Template Editor - Custom Theme TXT Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

As you make your changes, click the green “Update” button in the upper left corner to save them. Once those changes are saved, you can use the buttons on the right to preview your changes, send a test email, or restore the original template content.

Need examples for how to customize your new theme templates? Have a look at the [Customizing MailBeez Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)

### Editing Custom Layout Style Templates

Once you’ve created your custom layout style templates using the Customizing MailBeez Premium Email Templates tutorial, it is safe to begin with your custom edits. Customizing layout style templates can be done in just a few easy steps:

#### Select a Custom Layout Style to Edit

Using the custom layout style “myfriendly” within the Review Reminder Advanced module as an example, navigate to **admin > MailBeez > MailBeez Modules tab > Review Reminder Advanced module:**

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_config_panel.png&w=175&h=367&zc=1&q=100 "Review Reminder Advanced Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_config_panel.png "Review Reminder Advanced Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Click on the “Edit” button at the top of the configuration panel to access your configuration options:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/layout_style_selector.png&w=175&h=108&zc=1&q=100 "Review Reminder Advanced Layout Style Selector")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/layout_style_selector.png "Review Reminder Advanced Layout Style Selector")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Select the new custom layout style template, for example “**myfriendly**“, and click the “Update” button.

#### Launch Template Manager’s Template Editor

Remember “myfriendly\_body\_html\_step\_1″, “myfriendly\_body\_html\_step\_2″, etc from the Customizing MailBeez Premium Email Templates tutorial?

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/body_myfriendly.png&w=270&h=136&zc=1&q=100 "Custom Layout Style Body Templates")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/body_myfriendly.png "Custom Layout Style Body Templates")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Each of these layout style body sub-templates corresponds to an email cycle for its module. Looking at the Review Reminder Advanced module on the list of installed templates, notice just below it are some email cycle options (Initial Invitation, First Reminder, etc).

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png&w=270&h=46&zc=1&q=100 "Review Reminder Advanced Module Email Cycles")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png "Review Reminder Advanced Module Email Cycles")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Click on the first email cycle option to display it’s configuration panel, and then click on the Template Manager “Edit” button:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png&w=175&h=49&zc=1&q=100 "Review Reminder - Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png "Review Reminder - Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

#### Load the Custom Layout Style Templates

In the template editor, you’ll notice that the templates which are automatically loaded are the last templates you were editing (or the default layout style templates if this is your first time using Template Manager).

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review.png&w=270&h=131&zc=1&q=100 "Template Manager - Template Editor")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review.png "Template Manager - Template Editor")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**To load the new custom layout style template files, you must click the “Restore” button.** This has the dual function of both loading your custom templates, and also restoring the the previous templates to their original state.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/restore_button.png&w=175&h=262&zc=1&q=100 "Template Editor Restore Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/restore_button.png "Template Editor Restore Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

This is why it was so important to first make a set of custom templates before getting started because if you had made edits to the default templates, and then later came here to edit a new custom template, you would have lost all of the customizations you made to the default template.

#### Edit the Custom Layout Style Templates

In the Template Manager’s template editor, you can edit both the HTML and TXT templates, preview how the changes appear in the templates, send a test email, or restore your templates back to their original content if you break something or just want to undo all of your changes.

In the HTML template editor, you can customize images, text, style, layout and content:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_html.png&w=270&h=120&zc=1&q=100 "Template Editor - Review Reminder Advanced HTML template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_html.png "Template Editor - Review Reminder Advanced HTML template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In the TXT template editor, you can customize text, add or remove template variables, and determine the order in which text & template variables will appear in the email:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_txt.png&w=270&h=183&zc=1&q=100 "Template Editor - Review Reminder Advanced TXT template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_txt.png "Template Editor - Review Reminder Advanced TXT template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

As you make your changes, click the green “Update” button in the upper left corner to save them. Once those changes are saved, you can use the buttons on the right to preview your changes, send a test email, or restore the original template content.

#### Repeat the Process for Each Sub-Template

Again, staying with the custom layout style “myfriendly” within the Review Reminder Advanced module, just follow the same steps you used with the first sub-template:

- Navigate to **admin > MailBeez > MailBeez Modules tab > Review Reminder Advanced module** and click on it
- Click on the next email cycle option to bring up it’s configuration panel
- Click on the “Template Manager Edit” button
- Click the “Restore” button
- Edit the html and text sub-templates
- Click Update

Need examples for how to customize your new layout style templates? Have a look at the [Customizing MailBeez Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)

## Backing Up Your Customizations

Once you have completed your customizations, it is crucial that you create backups of your customized template (.tpl) files. Keeping a back up copy ensures you will be able to easily restore them if the need arises.

Customizations completed in the template editor of the Template Manager and Multilanguage Extension with Template Manager modules are stored in the database, not the template files. This is so the integrity of the original template files is protected in case they need to be restored in the event that a template gets broken during the customization process.

When you switch between layout style templates and then go in to the template editor to make your changes, the “Restore” button is used to load the template file for the layout style you just switched to. If you haven’t copied your customizations to the custom template files you created, the customizations stored in the database will be overwritten by the template file’s original content.

For this reason, **it is necessary to copy your customizations to your custom template files once you have completed your changes and *before* switching between templates.**.

Using the custom layout style “myfriendly” within the Review Reminder Advanced module as an example, here are some step-by-step instructions to help you through the process:


1. Navigate to **admin > MailBeez > MailBeez Modules tab > Review Reminder Advanced module** and click on it to display the the email cycle options which utilize the body sub-templates:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png&w=270&h=46&zc=1&q=100 "Review Reminder Advanced Module Email Cycles")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png "Review Reminder Advanced Module Email Cycles")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


1. Click on the first email cycle option to display it’s configuration panel, and then click on the Template Manager “Edit” button:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png&w=175&h=49&zc=1&q=100 "Review Reminder - Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png "Review Reminder - Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


1. Copy the contents of the HTML editor:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_html.png&w=270&h=120&zc=1&q=100 "Template Editor - Review Reminder Advanced HTML template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_html.png "Template Editor - Review Reminder Advanced HTML template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


1. Paste the contents of the HTML editor to its associated template file on your local drive, in this case: /mailhive/mailbeez/review\_advanced/email/myfriendly\_body\_html\_step1.tpl
2. Upload the file to the appropriate directory on your server, in this case: /mailhive/mailbeez/review\_advanced/email/
3. Return to the template editor in the first email cycle option and click the “Restore” button and then the “Update” button. Your customizations have now been saved to the database and cannot be accidentally overwritten with the restore functionality in the future.
4. Return to **MailBeez Modules tab > Review Reminder Advanced module** and click on the second email cycle option to display it’s configuration panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png&w=270&h=46&zc=1&q=100 "Review Reminder Advanced Module Email Cycles")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png "Review Reminder Advanced Module Email Cycles")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


1. Click on the Template Manager “Edit” button

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png&w=175&h=49&zc=1&q=100 "Review Reminder - Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png "Review Reminder - Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Copy the contents of the HTML editor
2. Paste the contents of the HTML editor to its associated template file on your local drive, in this case: /mailhive/mailbeez/review\_advanced/email/myfriendly\_body\_html\_step2.tpl
3. Upload the file to the appropriate directory on your server, in this case: /mailhive/mailbeez/review\_advanced/email/
4. Return to the template editor in the second email cycle option and click the “Restore” button and then the “Update” button. Your customizations have now been saved to the database and cannot be accidentally overwritten with the restore functionality in the future.
5. Repeat this process with any remaining email cycle options

**Failure to follow these steps will result in customized files being overwritten by the originals**

You will need to repeat this process for all of your customized layout style templates and body sub-templates for each premium module, as well as your customized theme templates.

## Using Template Manager With Free Email Templates

**Before you begin using Template Manager to edit your free email templates, you must create a backup of the original templates that came pre-installed with the free email modules so you can restore the templates if you break something during customization.**

**An overview of global vs.individual module customizations, as well as step-by-step instructions for creating custom templates, customizing the html code in the templates, & backing up your customizations can be found in the [Customizing MailBeez Free Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-free-email-templates/)**

### Editing the Common Main Templates

Navigate to **admin > MailBeez > MailBeez Configuration tab > Template Manager module** and click on the Common Main Template “Edit” button to access the Common Main templates in the template editor:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor.png&w=270&h=128&zc=1&q=100 "Template Manager - Template Editor")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor.png "Template Manager - Template Editor")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

From here, you can edit both the Common HTML and the Common TXT templates, preview how the changes appear in the templates, send a test email, or restore your templates back to their original content if you break something or just want to undo all of your changes.

**Warning! Clicking the “Restore” button will restore both templates to their original content! Back up any changes you want to save before clicking this button!**

In the HTML template editor, you can customize images, text, style, layout and content:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_html.png&w=270&h=106&zc=1&q=100 "Template Editor - Common HTML Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_html.png "Template Editor - Common HTML Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In the TXT template editor, you can customize text, add or remove template variables, and determine the order in which text & template variables will appear in the email:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_txt.png&w=175&h=120&zc=1&q=100 "Template Editor - Common TXT Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_txt.png "Template Editor - Common TXT Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

As you make your changes, click the green “Update” button in the upper left corner to save them. Once those changes are saved, you can use the buttons on the right to preview your changes, send a test email, or restore the original template content.

**Once you complete customizations of your Common Main templates, you must make back up copies for later use in the event that you update MailBeez or restore your original templates (which overwrites your customizations).**

### Editing Individual Module Templates

Using the Birthday Greetings module as an example, navigate to **admin > MailBeez > MailBeez Modules tab > Birthday Greetings module** and click on the Template Manager “Edit” button in the Birthday Greetings configuration panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png&w=175&h=49&zc=1&q=100 "Birthday Greetings - Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png "Birthday Greetings - Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Notice that the template editor looks and acts the same as it did for the Common Main template:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday.png&w=270&h=131&zc=1&q=100 "Template Manager - Template Editor")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday.png "Template Manager - Template Editor")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In the HTML template editor, you can customize images, text, style, layout and content just as you did with the Common Main template. The only difference here is that there is now a subject line that you can edit in addition to the body content:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_html.png&w=270&h=120&zc=1&q=100 "Template Editor - Birthday Greetings HTML Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_html.png "Template Editor - Birthday Greetings HTML Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The same is also true for the TXT template editor. Just as you did for the Common Main template, you can customize text, add or remove template variables, and determine the order in which text & template variables will appear in the Birthday Greetings email:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_txt.png&w=175&h=121&zc=1&q=100 "Template Editor - Birthday Greetings TXT Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_txt.png "Template Editor - Birthday Greetings TXT Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

This commonality of use and function across all templates for all free modules makes Template Manager super easy to learn and use as you work to customize all of your email templates!

**As with the Common Main templates, once you complete customizations of your various module templates, you must make back up copies for later use in the event that you update your modules or restore your original templates. Remember that using the “Restore” button to restore your original templates overwrites your customizations.**

## Backing Up Your Customizations

Once you have completed your customizations, it is crucial that you create backups of your customized template (.tpl) files for two reasons:

- Custom file names are the same as the default file names, so when you update your MailBeez framework and email modules as new versions are released, you could easily overwrite your customizations without thinking.
- Customizations completed in the template editor of the Template Manager are stored in the database, not in the template files, in order to protect the integrity of the original template files. The “Restore” functionality built in to the Template Manager will overwrite your customizations when the “Restore” button is clicked if those customizations aren’t saved to the template file.

For these reasons, **it is necessary to copy your customizations to your custom template files once you have completed your changes.**. Here’s how you do it, step-by-step.


1. Using the Birthday Greetings module as an example, navigate to **admin > MailBeez > MailBeez Modules tab > Birthday Greetings module** and click on the Template Manager “Edit” button in the Birthday Greetings configuration panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png&w=175&h=49&zc=1&q=100 "Birthday Greetings - Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_edit_button.png "Birthday Greetings - Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


1. Copy the contents of the HTML editor:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_html.png&w=270&h=120&zc=1&q=100 "Template Editor - Birthday Greetings HTML Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_html.png "Template Editor - Birthday Greetings HTML Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


1. Paste the contents of the HTML editor to its associate template file on your local drive, in this case: /mailhive/mailbeez/birthday/email/body\_html.tpl
2. Upload the file to the appropriate directory on your server, in this case: /mailhive/mailbeez/birthday/email/
3. Repeat the process for the TXT template by copying the contents of the TXT editor:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_txt.png&w=175&h=121&zc=1&q=100 "Template Editor - Birthday Greetings TXT Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_txt.png "Template Editor - Birthday Greetings TXT Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

1. Paste the contents of the TXT editor to its associated template file on your local drive, in this case: /mailhive/mailbeez/birthday/email/body\_txt.tpl
2. Upload the file to the appropriate directory on your server, in this case: /mailhive/mailbeez/birthday/email/
3. Return to the template editor in the Birthday Greeting module and click the “Restore” button and then the “Update” button. Your customizations have now been saved to the database and cannot be accidentally overwritten with the restore functionality in the future.
4. Repeat these steps with your Common Main templates and the individual templates of each of your free modules



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.
