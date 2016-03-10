---
# http://learn.getgrav.org/content/headers
title: The Google Analytics Dashboard Widget
slug: google-analytics-dashboard-widget-tutorial
# menu: The Google Analytics Dashboard Widget
date: 17-10-2012
published: true
publish_date: 17-10-2012
# unpublish_date: 17-10-2012
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

(English)

## Using the Google Analytics Dashboard Widget

Due to changes Google has made to the Google Analytics API, the way the MailBeez Google Analytics Dashboard Widget works has changed. There is a new process that must be followed in order for your widget to access & display your Google Analytics data.

We have created a step-by-step tutorial for you to make it easier.

**IMPORTANT:** Make sure you use the “old” Layout of Google Analytics

### Step 1: Set up the Google API Project

1. Navigate to: <https://code.google.com/apis/console/> and sign in to your Google account
2. If this is your first time here, a “Create Project” button will appear. Click it:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/create_project_button.png&w=270&h=252&zc=1&q=100 "Create Project Button")](http://www.mailbeez.com/images/doc/ga_dash_config/create_project_button.png "Create Project Button")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

4. Otherwise, you will see that the Google API Services Console is displayed. Select “Services” from the menu at left and check Analytics API from the API list:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/api_services_console.png&w=270&h=145&zc=1&q=100 "API Services Console - Services List")](http://www.mailbeez.com/images/doc/ga_dash_config/api_services_console.png "API Services Console - Services List")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

**Note:** You may get a Terms of Use popup if this is your first time here. If so, accept the terms and continue to the next step.

7. Select “API Access” from the menu at left to display the Google API Access Console:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/api_access_console1.png&w=270&h=140&zc=1&q=100 "API Access Console - Create Client ID")](http://www.mailbeez.com/images/doc/ga_dash_config/api_access_console1.png "API Access Console - Create Client ID")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

9. Click on the “Create an OAuth 2.0 client ID” button to bring up the “Create Client ID” popup window:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/create_client_id_popup1.png&w=270&h=160&zc=1&q=100 "Create Client ID - Step 1")](http://www.mailbeez.com/images/doc/ga_dash_config/create_client_id_popup1.png "Create Client ID - Step 1")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

11. In the “Product name” field, enter “MailBeez Application” (without the quotes)
12. Check the “Google Account” field. It should be pre-populated with your gmail address
13. Click the “Next” button to display the next screen:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/create_client_id_popup2.png&w=270&h=181&zc=1&q=100 "Create Client ID - Step 2")](http://www.mailbeez.com/images/doc/ga_dash_config/create_client_id_popup2.png "Create Client ID - Step 2")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

15. Select “Web application” (since PHP is mostly used for web applications). Use localhost or a domain if you would like to try it out
16. Click on “More Options”
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/create_client_id_popup3.png&w=270&h=202&zc=1&q=100 "Create Client ID - Step 3")](http://www.mailbeez.com/images/doc/ga_dash_config/create_client_id_popup3.png "Create Client ID - Step 3")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

18. Change the value for Authorized Redirect URIs – remove “https://www.example.com/oauth2callback” and replace it with the URL shown in your Google Analytics Dashboard Widget
19. Click on “Create client ID”
20. The API Setup is now complete and the information you need to configure your dashboard widget is visible:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/api_access_console2.png&w=270&h=212&zc=1&q=100 "API Access Console - Setup Complete")](http://www.mailbeez.com/images/doc/ga_dash_config/api_access_console2.png "API Access Console - Setup Complete")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

22. To complete the next step, you will need the Client ID and the Client Secret from this screen

### Step 2: Configure the Dashboard Widget

1. Navigate to the Google Analytics Dashboard Widget on your MailBeez Dashboard:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/ga_dash_config1.png&w=270&h=96&zc=1&q=100 "Google Analytics Dashboard Widget")](http://www.mailbeez.com/images/doc/ga_dash_config/ga_dash_config1.png "Google Analytics Dashboard Widget")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

3. Enter the the Client ID and the Client Secret from the Google API Console & click the “Confirm” button
4. Click the “Connect” button to connect your widget to your Google account:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/ga_dash_config2.png&w=270&h=95&zc=1&q=100 "Connect to Google")](http://www.mailbeez.com/images/doc/ga_dash_config/ga_dash_config2.png "Connect to Google")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

6. If you’re not signed in to your Google account, you will be redirected to a Google login screen. Enter your login information to be redirected to the Google Authentication screen.
7. If you are already logged in to your Google account, you will be immediately redirected to the Google authentication screen:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/ga_authentication.png&w=270&h=79&zc=1&q=100 "Google Analytics Authentication Screen")](http://www.mailbeez.com/images/doc/ga_dash_config/ga_authentication.png "Google Analytics Authentication Screen")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

9. Click the “Allow Access” button and you’ll be redirected back to your MailBeez Dashboard, where a list of your Google Account Profiles will display in the widget. Select the one you want to use:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/ga_dash_config3.png&w=270&h=94&zc=1&q=100 "Your Google Account Profiles")](http://www.mailbeez.com/images/doc/ga_dash_config/ga_dash_config3.png "Your Google Account Profiles")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)

11. Once you select the Google Account Profile, the Google Analytics-O-Pie will be displayed:
[![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/lib/scripts/timthumb/thumb.php?src=http://www.mailbeez.com/images/doc/ga_dash_config/ga_dash_widget.png&w=270&h=116&zc=1&q=100 "Google Analytics-O-Pie")](http://www.mailbeez.com/images/doc/ga_dash_config/ga_dash_widget.png "Google Analytics-O-Pie")![](http://localhost/wordpress_mailbeez_EOL/wp-content/themes/awake/images/shortcodes/image_shadow.png)


If you prefer, you may instead configure this widget by clicking the “config” link beneath the widget, or by navigating to Configuration tab > Dashboard Configuration > Google Analytics-O-Pie  
  
