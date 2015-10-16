---
# http://learn.getgrav.org/content/headers
title: The Google Analytics O'Pie
slug: dashboard_ga
# menu: The Google Analytics O'Pie
date: 07-05-2012
published: true
publish_date: 07-05-2012
# unpublish_date: 07-05-2012
template: docs
# theme: false
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: done
    category: [docs]
    tag: [core]
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


Delivered with the MailBeez framework, the Google-Analytics-O-Pie is a powerful widget that provides you with a visual report in the form of a pie chart of all the MailBeez activity data that Google Analytics tracks for you, such as site visits resulting from MailBeez email campaigns, revenue earned with MailBeez, and a breakdown of that revenue by module so that you can see which modules are working hardest for you!

![](Screen_ga_dash_widget.png "Google Analytics-O-Pie")

>>>>>You must have a Google Analytics account set up and have it activated & configured in MailBeez for this widget to function.
 

#### Common Questions

**Why does the Google Analytics data differ from MailBeez Analytics data?**

Google Analytics can only track orders made after clicking a direct link in a MailBeez generated email, so for example, if a customer receives a MailBeez coupon email on his mobile device, but then later places his order using his desktop computer by simply typing in the discount code from the email, the Google Analytics connection to the MailBeez Email is lost.

Conversely, any orders made using MailBeez generated coupons will be tracked by MailBeez Analytics whether the customer clicks the link in the email or manually enters the coupon code from the email during checkout.

**Why do I have such few clicks recorded in Google Analytics?**

Some stores do not have Google Analytics tracking on their store-front. When your MailBeez emails contain a link to the store-front, these visits, (and the resulting purchases), won’t be recorded by Google Analytics.  
  


## Using the Google Analytics Dashboard Widget

Due to changes Google has made to the Google Analytics API, the way the MailBeez Google Analytics Dashboard Widget works has changed. There is a new process that must be followed in order for your widget to access & display your Google Analytics data.

We have created a step-by-step tutorial for you to make it easier.

>>>>Make sure you use the “old” Layout of Google Analytics

### Step 1: Set up the Google API Project

1. Navigate to: <https://code.google.com/apis/console/> and sign in to your Google account

2. If this is your first time here, a “Create Project” button will appear. Click it:
![](Screen_create_project_button.png "Create Project Button")

4. Otherwise, you will see that the Google API Services Console is displayed. Select “Services” from the menu at left and check Analytics API from the API list:
![](Screen_api_services_console.png "API Services Console - Services List")  
 **Note:** You may get a Terms of Use popup if this is your first time here. If so, accept the terms and continue to the next step.

7. Select “API Access” from the menu at left to display the Google API Access Console:
![](Screen_api_access_console1.png "API Access Console - Create Client ID")

9. Click on the “Create an OAuth 2.0 client ID” button to bring up the “Create Client ID” popup window:
![](Screen_create_client_id_popup1.png "Create Client ID - Step 1")

11. In the “Product name” field, enter “MailBeez Application” (without the quotes)

12. Check the “Google Account” field. It should be pre-populated with your gmail address

13. Click the “Next” button to display the next screen:
![](Screen_create_client_id_popup2.png "Create Client ID - Step 2")

15. Select “Web application” (since PHP is mostly used for web applications). Use localhost or a domain if you would like to try it out

16. Click on “More Options”
![](Screen_create_client_id_popup3.png "Create Client ID - Step 3")


18. Change the value for Authorized Redirect URIs – remove “https://www.example.com/oauth2callback” and replace it with the URL shown in your Google Analytics Dashboard Widget

19. Click on “Create client ID”

20. The API Setup is now complete and the information you need to configure your dashboard widget is visible:
![](Screen_api_access_console2.png "API Access Console - Setup Complete")


22. To complete the next step, you will need the Client ID and the Client Secret from this screen

### Step 2: Configure the Dashboard Widget

1. Navigate to the Google Analytics Dashboard Widget on your MailBeez Dashboard:
![](Screen_ga_dash_config1.png "Google Analytics Dashboard Widget")


3. Enter the the Client ID and the Client Secret from the Google API Console & click the “Confirm” button

4. Click the “Connect” button to connect your widget to your Google account:
![](Screen_ga_dash_config2.png "Connect to Google")


6. If you’re not signed in to your Google account, you will be redirected to a Google login screen. Enter your login information to be redirected to the Google Authentication screen.

7. If you are already logged in to your Google account, you will be immediately redirected to the Google authentication screen:
![](Screen_ga_authentication.png "Google Analytics Authentication Screen")


9. Click the “Allow Access” button and you’ll be redirected back to your MailBeez Dashboard, where a list of your Google Account Profiles will display in the widget. Select the one you want to use:
![](Screen_ga_dash_config3.png "Your Google Account Profiles")


11. Once you select the Google Account Profile, the Google Analytics-O-Pie will be displayed:
![](Screen_ga_dash_widget.png "Google Analytics-O-Pie")



If you prefer, you may instead configure this widget by clicking the “config” link beneath the widget, or by navigating to Configuration tab > Dashboard Configuration > Google Analytics-O-Pie  