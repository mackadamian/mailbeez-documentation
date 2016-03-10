---
# http://learn.getgrav.org/content/headers
title: Multilanguage Extension with Template Manager
slug: multilanguage-extension-with-template-manager
# menu: Multilanguage Extension with Template Manager
date: 24-08-2012
published: true
publish_date: 24-08-2012
# unpublish_date: 24-08-2012
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

The Multilanguage Extension provides compatible online stores with the tools to make a hassle free, fast and easy entry into the world of internationalization, by enabling all existing and future MailBeez Modules (even your own as long as they use MailBeez template system), to support multiple language input.

With that taken care of, all that is left for you to do is to translate your email text into the additional languages, (and with tools like mygengo, this could not be easier), copy it into the module’s admin, and away you go.

**If you are using this module, it is assumed that you already have multiple language functionality set up in your store. If you have not yet done so, please do so before installing this module. See your e-commerce platform’s documentation for assistance on setting up multiple languages in your store.**

## Getting Started

1. Log in to your store’s admin interface
2. Navigate to your MailBeez interface and click on the Configuration tab
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/common_images/config_tab2.png&w=270&h=175&zc=1&q=100 "Configuration Tab")](http://www.mailbeez.com/images/doc/common_images/config_tab2.png "Configuration Tab")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Locate the Multilanguage Extension with Template Manager module and click on it.
5. Click on the “Install” button to install the configuration settings into your database:  
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_install.png&w=175&h=78&zc=1&q=100 "Install Configuration Settings into your Database")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_install.png "Install Configuration Settings into your Database")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The configuration panel is now visible:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_config_panel_locked.png&w=175&h=224&zc=1&q=100 "Multilanguage Extension Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_config_panel_locked.png "Multilanguage Extension Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

 

## Configuring Multilanguage Extension with Template Manager

### Unlock the Module

There are 2 “Edit” buttons in the configuration panel, as shown in the image above.

1. Click on second “Edit” button at the bottom of the configuration panel
2. Enter your personal certificate key that came with the module delivery email from Avangate & click the “Update” button

Your module is now unlocked and ready for configuration.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_config_panel_unlocked.png&w=175&h=328&zc=1&q=100 "Unlocked Multilanguage Extension Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_config_panel_unlocked.png "Unlocked Multilanguage Extension Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

### Configure General Settings

Click the first “Edit” button at the top of the configuration panel to access the general settings. There are 2 of them:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_general_settings.png&w=175&h=157&zc=1&q=100 "Multilanguage Extension General Settings")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_general_settings.png "Multilanguage Extension General Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Activate Module**  
 This setting turns the module on and off. It is set to “True” by default, meaning the module is on and ready to work. Change this setting to “False” to deactivate the module and disable it from being used.

**Select Your Template Theme**  
 This setting lets you choose which template theme you want to use. By default, it is set to “Default”, meaning it will use the template theme that came pre-installed with your MailBeez software.

When you have completed your configurations, click the “Update button”.

### Configure the Language Settings

Next, you need to set up your language configuration settings. Click on the “Configure” button in the “Configure Languages” section of the module’s configuration panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/config_language_button.png&w=175&h=51&zc=1&q=100 "Configure Language Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/config_language_button.png "Configure Language Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The “Detected Languages” and “Detected Countries” areas of the language configuration panel each have drop down lists that are populated with all of the languages you have set up in your store:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/language_configuration.png&w=270&h=116&zc=1&q=100 "Multilanguage Extension Language Configuration Settings")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/language_configuration.png "Multilanguage Extension Language Configuration Settings")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

During the language detection process that takes place when a module is run, the plugin uses these two different approaches to try and determine the customer’s language based on the settings you assign here.

**Detected Languages**  
 In this area, you will see the unique strings for the Order Totals terminology in various languages. For example, in English, you would see “sum” and in German you would see “gesamt”. The drop down list here allows you to map those strings to a language.

**Detected Countries**  
 In this area, you can configure which languages you want to map to each country. Simply use the drop down list to make your selections.

When you’ve completed your configurations, click the green “Update” button in the upper left corner to save your new settings. Configuration of the module is now complete!

 

## How Do I Use the Multilanguage Template Manager?

The processes for using the Multilanguage Template Manager to edit & customize your email templates are slightly different between MailBeez premium email templates and MailBeez free email templates because MailBeez premium email modules provide you with many more options than do MailBeez free email modules.

For example, MailBeez free email modules allow for a single theme in multiple languages (utilizing the Common Main templates) and a single layout style in multiple languages (utilizing each module’s body\_html.tpl file), whereas MailBeez premium email modules allow for multiple themes and layout styles, as well as the ability to create custom versions of each in multiple languages and switch between them as desired.

For this reason, we have separated these processes into two different sections within this tutorial for easier use & understanding.

 

## Using the Multilanguage Template Manager With Premium Email Templates

**Before you begin using the Multilanguage Template Manager to edit your premium email templates, you must create custom templates rather than making edits directly to the templates that came pre-installed with MailBeez and your Premium MailBeez modules to avoid losing your customizations when using the Multilanguage Template Manager to switch between templates.**

This is because the Multilanguage Template Manager is designed to protect the integrity of the original templates that come pre-installed with MailBeez and your Premium MailBeez modules. If a template gets broken during editing, you can restore the originals and start over. This functionality also comes in to play when you switch between templates, so if you don’t have custom templates set up, edits you make to the original files will be lost.

**An overview of theme templates vs. layout style templates, as well as step-by-step instructions for creating custom templates & backing up your customizations can be found in the [Customizing MailBeez Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)**

### Editing Custom Theme Templates

Once you’ve created your custom theme templates using the Customizing MailBeez Premium Email Templates tutorial, it is safe to begin with your custom edits. Customizing theme templates can be done in just a few easy steps:

#### Select a Custom Theme to Edit

Using the custom theme you created, for example “**mydefault**“, navigate to ** admin > MailBeez > Configuration tab > Multilanguage Extension with Template Manager module:**

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_config_panel_unlocked.png&w=175&h=328&zc=1&q=100 "Unlocked Multilanguage Extension Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_config_panel_unlocked.png "Unlocked Multilanguage Extension Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Click on the “Edit” button at the top of the configuration panel to access your configuration options:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/theme_selector.png&w=175&h=107&zc=1&q=100 "Multilanguage Template Manager Configuration Settings - Theme Selector")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/theme_selector.png "Multilanguage Template Manager Configuration Settings - Theme Selector")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Select the new custom theme template you created, for example “**mydefault**“, and click the “Update” button.

#### Launch Multilanguage Template Manager’s Template Editor

Remembering from the Customizing MailBeez Premium Email Templates tutorial that Theme templates and Common Main templates are in fact one in the same, click on the Common Main Template “Edit” button on the Multilanguage Template Manager configuration panel to access the Common Main templates in the template editor:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor.png&w=270&h=129&zc=1&q=100 "Multilanguage Template Manager - Template Editor")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor.png "Multilanguage Template Manager - Template Editor")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Notice in the image above that the module has created tabs bearing the name of each language you have set up in your store, as well as its corresponding flag icon. These tabs contain custom language files created for you by Multilanguage Template Manager.

Their contents are exact replicas of the last templates you were editing (or the default templates if this is your first time using the module). The automatically created custom language templates are in your store’s default language and will remain so until you copy in your translated versions and click the “Update” button. More on that later.

#### Load the New Custom Theme Templates

To load the files for the new custom theme you selected in the first step, you must click the “Restore” button. This has the dual function of both loading your custom templates, and also **restoring the the previous templates to their original state.**

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_restore_button.png&w=175&h=278&zc=1&q=100 "Multilanguage Template Editor Restore Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_restore_button.png "Multilanguage Template Editor Restore Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

This is why it was so important to first make a set of custom templates before getting started because if you had made edits to the default templates, and then later came here to edit a new custom theme template, you would have lost all of the customizations you made to the default templates.

#### Edit the Custom Theme Templates

In the Multilanguage Template Manager’s template editor, you can edit both the HTML and TXT templates for each language, preview how the changes appear in the templates, send a test email, or restore your templates back to their original content if you break something or just want to undo **all** of your changes.

A really cool feature of the Multilanguage Template Manager is that when you click one of the language tabs at the top of the editor, the flags by each editable field all change to match the language you selected!

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags1.png&w=270&h=298&zc=1&q=100 "Multilanguage Template Editor - Language Indicators")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags1.png "Multilanguage Template Editor - Language Indicators")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

This feature makes it much easier to know at a glance which language template you’re editing when you’re clicking about here and there getting things all set up.

In the HTML template editor, you can customize images, text, style, layout and content:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_html.png&w=270&h=106&zc=1&q=100 "Multilanguage Template Editor - Custom Theme HTML Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_html.png "Multilanguage Template Editor - Custom Theme HTML Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In the TXT template editor, you can customize text, add or remove template variables, and determine the order in which text & template variables will appear in the email:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_txt.png&w=175&h=120&zc=1&q=100 "Multilanguage Template Editor - Custom Theme TXT Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_txt.png "Multilanguage Template Editor - Custom Theme TXT Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

As you make your changes, click the green “Update” button in the upper left corner to save them. Once those changes are saved, you can use the buttons on the right to preview your changes, send a test email, or restore the original template content.

Once you’ve finalized your templates in your default language, all that’s left to do is translate them into each language you wish to use and copy those translations into the custom language templates the module created for you. Simply click on the language tabs across the top to access the templates for each language.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags2.png&w=270&h=90&zc=1&q=100 "Multilanguage Template Editor - Language Tabs")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags2.png "Multilanguage Template Editor - Language Tabs")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Need examples for how to customize your new theme templates? Have a look at the [Customizing MailBeez Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)

### Editing Custom Layout Style Templates

Once you’ve created your custom layout style templates using the Customizing MailBeez Premium Email Templates tutorial, it is safe to begin with your custom edits. Customizing layout style templates can be done in just a few easy steps:

#### Select a Custom Layout Style to Edit

Using the custom layout style “myfriendly” within the Review Reminder Advanced module as an example, navigate to **admin > MailBeez > MailBeez Modules tab > Review Reminder Advanced module:**

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_config_panel.png&w=175&h=367&zc=1&q=100 "Review Reminder Advanced Configuration Panel")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_config_panel.png "Review Reminder Advanced Configuration Panel")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Click on the “Edit” button at the top of the configuration panel to access your configuration options:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/layout_style_selector.png&w=175&h=108&zc=1&q=100 "Review Reminder Advanced Layout Style Selector")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/layout_style_selector.png "Review Reminder Advanced Layout Style Selector")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Select the new custom layout style template, for example “**myfriendly**“, and click the “Update” button.

#### Launch the Multilanguage Template Manager’s Template Editor

Remember “myfriendly\_body\_html\_step\_1″, “myfriendly\_body\_html\_step\_2″, etc from the Customizing MailBeez Premium Email Templates tutorial?

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/body_myfriendly.png&w=270&h=136&zc=1&q=100 "Custom Layout Style Body Templates")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/body_myfriendly.png "Custom Layout Style Body Templates")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Each of these layout style body sub-templates corresponds to an email cycle for its module. Looking at the Review Reminder Advanced module on the list of installed templates, notice just below it are some email cycle options (Initial Invitation, First Reminder, etc).

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png&w=270&h=46&zc=1&q=100 "Review Reminder Advanced Module Email Cycles")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png "Review Reminder Advanced Module Email Cycles")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Click on the first email cycle option to display it’s configuration panel, and then click on the Multilanguage Template Manager “Edit” button:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png&w=175&h=55&zc=1&q=100 "Review Reminder - Multilanguage Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png "Review Reminder - Multilanguage Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

#### Load the Custom Layout Style Templates

Notice in the image below that, just as it was with the custom theme templates, the module has created language tabs for each of your store’s languages and a custom language template in each of those languages. Just as with the custom theme templates, these custom language files are awaiting your translations.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_review.png&w=270&h=131&zc=1&q=100 "Multilanguage Template Manager - Template Editor")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_review.png "Multilanguage Template Manager - Template Editor")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

To load the new custom layout style template files, you must click the “Restore” button. This has the dual function of both loading your custom templates, and also **restoring the the previous templates to their original state.**

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_restore_button.png&w=175&h=278&zc=1&q=100 "Multilanguage Template Editor Restore Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_restore_button.png "Multilanguage Template Editor Restore Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

This is why it was so important to first make a set of custom templates before getting started because if you had made edits to the default templates, and then later came here to edit a new custom template, you would have lost all of the customizations you made to the default template.

#### Edit the Custom Layout Style Templates

Just as with the custom theme templates, you can edit both the HTML and TXT templates for each language, preview how the changes appear in the templates, send a test email, or restore your templates back to their original content if you break something or just want to undo **all** of your changes.

In the HTML template editor, you can customize images, text, style, layout and content:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_html.png&w=270&h=120&zc=1&q=100 "Multilanguage Template Editor - Review Reminder Advanced HTML template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_html.png "Multilanguage Template Editor - Review Reminder Advanced HTML template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In the TXT template editor, you can customize text, add or remove template variables, and determine the order in which text & template variables will appear in the email:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_txt.png&w=270&h=183&zc=1&q=100 "Multilanguage Template Editor - Review Reminder Advanced TXT template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_txt.png "Multilanguage Template Editor - Review Reminder Advanced TXT template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

As you make your changes, click the green “Update” button in the upper left corner to save them. Once those changes are saved, you can use the buttons on the right to preview your changes, send a test email, or restore the original template content.

Once you’ve finalized your templates in your default language, all that’s left to do is translate them into each language you wish to use and copy those translations into the custom language templates the module created for you. Simply click on the language tabs across the top to access the templates for each language.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags2.png&w=270&h=90&zc=1&q=100 "Multilanguage Template Editor - Language Tabs")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags2.png "Multilanguage Template Editor - Language Tabs")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

#### Repeat the Process for Each Sub-Template

Just follow the same steps you used with the first sub-template:

- Navigate to **admin > MailBeez > MailBeez Modules tab > Review Reminder Advanced module** and click on it
- Click on the next email cycle option to bring up it’s configuration panel
- Click on the “Template Manager Edit” button
- Click the “Restore” button
- Edit the html and text sub-templates
- Translate the templates and copy them into the custom language templates
- Click Update

Need examples for how to customize your new layout style templates? Have a look at the [Customizing MailBeez Premium Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-premium-email-templates/)

 

## Backing Up Your Customizations

Once you have completed your customizations, it is crucial that you create backups of your customized template (.tpl) files. Keeping a back up copy ensures you will be able to easily restore them if the need arises.

Customizations completed in the template editor of the Template Manager are stored in the database, not the template files. This is so the integrity of the original template files is protected in case they need to be restored in the event that a template gets broken during the customization process.

When you switch between layout style templates and then go in to the template editor to make your changes, the “Restore” button is used to load the template file for the layout style you just switched to. If you haven’t copied your customizations to the custom template files you created, the customizations stored in the database will be overwritten by the template file’s original content.

For this reason, **it is necessary to copy your customizations to your custom template files once you have completed your changes and *before* switching between templates.**.

Using the custom layout style “myfriendly” within the Review Reminder Advanced module as an example, here are some step-by-step instructions to help you through the process:

1. Navigate to **admin > MailBeez > MailBeez Modules tab > Review Reminder Advanced module** and click on it to display the the email cycle options which utilize the body sub-templates:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png&w=270&h=46&zc=1&q=100 "Review Reminder Advanced Module Email Cycles")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png "Review Reminder Advanced Module Email Cycles")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Click on the first email cycle option to display it’s configuration panel, and then click on the Template Manager “Edit” button:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png&w=175&h=55&zc=1&q=100 "Review Reminder - Multilanguage Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png "Review Reminder - Multilanguage Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. Copy the contents of the HTML editor:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_html.png&w=270&h=120&zc=1&q=100 "Multilanguage Template Editor - Review Reminder Advanced HTML template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_review_html.png "Multilanguage Template Editor - Review Reminder Advanced HTML template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

7. Paste the contents of the HTML editor to its associated template file on your local drive, in this case: /mailhive/mailbeez/review\_advanced/email/myfriendly\_body\_html\_step1.tpl
8. Upload the file to the appropriate directory on your server, in this case: /mailhive/mailbeez/review\_advanced/email/
9. Return to the template editor in the first email cycle option and click the “Restore” button and then the “Update” button. Your customizations have now been saved to the database and cannot be accidentally overwritten with the restore functionality in the future.
10. Return to **MailBeez Modules tab > Review Reminder Advanced module** and click on the second email cycle option to display it’s configuration panel:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png&w=270&h=46&zc=1&q=100 "Review Reminder Advanced Module Email Cycles")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/review_reminder_email_cycles.png "Review Reminder Advanced Module Email Cycles")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

12. Click on the Template Manager “Edit” button
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png&w=175&h=55&zc=1&q=100 "Review Reminder - Multilanguage Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png "Review Reminder - Multilanguage Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

14. Copy the contents of the HTML editor
15. Paste the contents of the HTML editor to its associated template file on your local drive, in this case: /mailhive/mailbeez/review\_advanced/email/myfriendly\_body\_html\_step2.tpl
16. Upload the file to the appropriate directory on your server, in this case: /mailhive/mailbeez/review\_advanced/email/
17. Return to the template editor in the second email cycle option and click the “Restore” button and then the “Update” button. Your customizations have now been saved to the database and cannot be accidentally overwritten with the restore functionality in the future.
18. Repeat this process with any remaining email cycle options

**Failure to follow these steps will result in customized files being overwritten by the originals**

You will need to repeat this process for all of your customized layout style templates and body sub-templates for each premium module, as well as your customized theme templates.

 

## Using the Multilanguage Template Manager With Free Email Templates

**Before you begin using the Multilanguage Template Manager to edit your free email templates, you must create a backup of the original templates that came pre-installed with the free email modules so you can restore the templates if you break something during customization.**

**An overview of global vs.individual module customizations, as well as step-by-step instructions for creating custom templates, customizing the html code in the templates, & backing up your customizations can be found in the [Customizing MailBeez Free Email Templates tutorial](/documentation/tutorials/customizing-mailbeez-free-email-templates/)**

### Editing the Common Main Templates

Navigate to **admin > MailBeez > MailBeez Configuration tab > Multilanguage Extension with Template Manager module** and click on the Common Main Template “Edit” button to access the Common Main templates in the template editor:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor.png&w=270&h=129&zc=1&q=100 "Multilanguage Template Manager - Template Editor")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor.png "Multilanguage Template Manager - Template Editor")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In the Multilanguage Template Manager’s template editor, you can edit both the HTML and TXT templates for each language, preview how the changes appear in the templates, send a test email, or restore your templates back to their original content if you break something or just want to undo **all** of your changes.

**Warning! Clicking the “Restore” button will restore both templates to their original content! Back up any changes you want to save before clicking this button!**

And just like with the premium email templates, a really cool feature of the Multilanguage Template Manager is that when you click one of the language tabs at the top of the editor, the flags by the Subject line, HTML template editor, and TXT template editor all change to match the language you selected.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags1.png&w=270&h=298&zc=1&q=100 "Multilanguage Template Editor - Language Indicators")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags1.png "Multilanguage Template Editor - Language Indicators")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

This feature makes it much easier to know at a glance which language template you’re editing when you’re clicking about here and there getting things all set up.

In the HTML template editor, you can customize images, text, style, layout and content:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_html.png&w=270&h=106&zc=1&q=100 "Multilanguage Template Editor - Common HTML Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_html.png "Multilanguage Template Editor - Common HTML Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In the TXT template editor, you can customize text, add or remove template variables, and determine the order in which text & template variables will appear in the email:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_txt.png&w=175&h=120&zc=1&q=100 "Multilanguage Template Editor - Common TXT Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_txt.png "Multilanguage Template Editor - Common TXT Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

As you make your changes, click the green “Update” button in the upper left corner to save them. Once those changes are saved, you can use the buttons on the right to preview your changes, send a test email, or restore the original template content.

Once you’ve finalized your templates in your default language, all that’s left to do is translate them into each language you wish to use and copy those translations into the custom language templates the module created for you. Simply click on the language tabs across the top to access the templates for each language.

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags2.png&w=270&h=90&zc=1&q=100 "Multilanguage Template Editor - Language Tabs")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_flags2.png "Multilanguage Template Editor - Language Tabs")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Once you complete customizations of your Common Main templates, you must make back up copies for later use in the event that you update MailBeez or restore your original templates (which overwrites your customizations).**

### Editing Individual Module Templates

Using the Birthday Greetings module as an example, navigate to **admin > MailBeez > MailBeez Modules tab > Birthday Greetings module** and click on the Multilanguage Template Manager “Edit” button in the Birthday Greetings configuration panel:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png&w=175&h=55&zc=1&q=100 "Birthday Greetings - Multilanguage Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png "Birthday Greetings - Multilanguage Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Notice that the template editor looks and acts the same as it did for the Common Main template:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_bday.png&w=270&h=131&zc=1&q=100 "Multilanguage Template Manager - Template Editor")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_editor_bday.png "Multilanguage Template Manager - Template Editor")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

In the HTML template editor, you can customize images, text, style, layout and content just as you did with the Common Main template. The only difference here is that there is now a subject line that you can edit in addition to the body content:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_html.png&w=270&h=120&zc=1&q=100 "Multilanguage Template Editor - Birthday Greetings HTML Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_html.png "Multilanguage Template Editor - Birthday Greetings HTML Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

The same is also true for the TXT template editor. Just as you did for the Common Main template, you can customize text, add or remove template variables, and determine the order in which text & template variables will appear in the Birthday Greetings email:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_txt.png&w=175&h=121&zc=1&q=100 "Multilanguage Template Editor - Birthday Greetings TXT Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_txt.png "Multilanguage Template Editor - Birthday Greetings TXT Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

This commonality of use and function across all templates for all free modules makes Template Manager super easy to learn and use as you work to customize all of your email templates!

As you make your changes, click the green “Update” button in the upper left corner to save them. Once those changes are saved, you can use the buttons on the right to preview your changes, send a test email, or restore the original template content.

Once you’ve finalized your templates in your default language, all that’s left to do is translate them into each language you wish to use and copy those translations into the custom language templates the module created for you. Simply click on the language tabs across the top to access the templates for each language.

**As with the Common Main templates, once you complete customizations of your various module templates, you must make back up copies for later use in the event that you update your modules or restore your original templates. Remember that using the “Restore” button to restore your original templates overwrites your customizations.**

 

## Backing Up Your Customizations

Once you have completed your customizations, it is crucial that you create backups of your customized template (.tpl) files for two reasons:

- Custom file names are the same as the default file names, so when you update your MailBeez framework and email modules as new versions are released, you could easily overwrite your customizations without thinking.
- Customizations completed in the template editor of the Template Manager are stored in the database, not in the template files, in order to protect the integrity of the original template files. The “Restore” functionality built in to the Template Manager will overwrite your customizations when the “Restore” button is clicked if those customizations aren’t saved to the template file.

For these reasons, **it is necessary to copy your customizations to your custom template files once you have completed your changes.**. Here’s how you do it, step-by-step.

1. Using the Birthday Greetings module as an example, navigate to **admin > MailBeez > MailBeez Modules tab > Birthday Greetings module** and click on the Template Manager “Edit” button in the Birthday Greetings configuration panel:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png&w=175&h=55&zc=1&q=100 "Review Reminder - Multilanguage Template Manager Edit Button")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_edit_button.png "Review Reminder - Multilanguage Template Manager Edit Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. This launches the template editor:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday.png&w=270&h=131&zc=1&q=100 "Multilanguage Template Manager - Template Editor")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday.png "Multilanguage Template Manager - Template Editor")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

5. Copy the contents of the HTML editor:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_html.png&w=270&h=120&zc=1&q=100 "Multilanguage Template Editor - Birthday Greetings HTML Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_html.png "Multilanguage Template Editor - Birthday Greetings HTML Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

7. Paste the contents of the HTML editor to its associated template file on your local drive, in this case: /mailhive/mailbeez/birthday/email/body\_html.tpl
8. Upload the file to the appropriate directory on your server, in this case: /mailhive/mailbeez/birthday/email/
9. Repeat the process for the TXT template by copying the contents of the TXT editor:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_txt.png&w=175&h=121&zc=1&q=100 "Multilanguage Template Editor - Birthday Greetings TXT Template")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr/tm_editor_bday_txt.png "Multilanguage Template Editor - Birthday Greetings TXT Template")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

11. Paste the contents of the TXT editor to its associated template file on your local drive, in this case: /mailhive/mailbeez/birthday/email/body\_txt.tpl
12. Upload the file to the appropriate directory on your server, in this case: /mailhive/mailbeez/birthday/email/
13. Return to the template editor in the Birthday Greeting module and click the “Restore” button and then the “Update” button. Your customizations have now been saved to the database and cannot be accidentally overwritten with the restore functionality in the future.
14. Repeat these steps with your Common Main templates and the individual templates of each of your free modules

 

## Running Email Modules With the Multilanguage Template Manager

There are two really cool features built into the Multilanguage Extension with Template Manager module that can be seen in both Simulation Mode and Production Mode.

Outside the Multilanguage Template Editor environment, the default buttons for “View html”, “View txt” and “Send Test-Mail” are automatically enhanced with a dialog box for selecting the language:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_choose_language.png&w=270&h=88&zc=1&q=100 "Multilanguage Template Manager - Language Selector")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_choose_language.png "Multilanguage Template Manager - Language Selector")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

Whilst running your Mailbeez email modules, this module enhances the output list with information about the detected language and the language detection method:

[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_run_popup.png&w=270&h=95&zc=1&q=100 "Multilanguage Template Manager - Run Results Popup")](http://www.mailbeez.com/images/doc/configbeez/mailbeez_pro_tmplmngr_lng/mletm_run_popup.png "Multilanguage Template Manager - Run Results Popup")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

With MailBeez, you can always be assured that your premium modules are fully integrated with, and extend their functionality throughout, the MailBeez framework!



## Run MailBeez Automatically

If you want MailBeez to run automatically, you have two options:

**1. [Set up a cronjob](/documentation/installation/config/advanced-configuration/)
2. [Install the simple and affordable Run MailBeez Automatically module](/documentation/configbeez/config_cron_simple/)
**
Without one of the above options in place, it will be up to you to manually send out your MailBeez emails by clicking the “Run” button in each module you want to run, as often as you want to run it. The Run MailBeez Automatically module is recommended because it is for most users the easiest option.
