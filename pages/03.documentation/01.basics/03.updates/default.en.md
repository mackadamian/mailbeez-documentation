---
# http://learn.getgrav.org/content/headers
title: Updating the MailBeez Core System
slug: updates
routes:
  default: /documentation/updates
  aliases:
    - /documentation/installation/config
  
menu: Updates
published: true
template: docs
# theme: false
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    category: docs
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


With Version 3.0 MailBeez contains a comfortable tool to keep your installation up to date!

## Update after receiving notification

The integrated version control will notify you when there is a new MailBeez version available. Please click on the notification and follow the steps in the update tool.

The update tool will perform the following steps:
1. Check server environment
1. Download new version
1. Check if all files are writable - this ensures that you won't get a "version mix" with old, not writable files
1. Backup of /mailhive directory
1. Write new files (all existing core files will be overwritten)

Upon returning to the MailBeez admin panel, you should see a new notification.

>>>>>>If you are facing issues with the Backup process not finishing, please delete all files that begin `appcache_` from the directory `/mailhive/common/templates_c` on the server hosting your shopping-cart system. With MailBeez Version 3.3.4 the cache is cleaned up automatically.


## Update manually

In some cases, it will be necessary to update manually using the update tool.

To do so please add

`?cloudloader_mode=update_core` 

to the URL of your MailBeez page, so the URL in your browser looks similar to:

`http://<shop-url>/<admin>/mailbeez.php?cloudloader_mode=update_core`

then follow the steps for updating the core system.


## Update using FTP

The updater is still not doing what it should? You can update "Old-School" style using FTP:

Please
[download the MailBeez Core System (.zip)](https://apps.mailbeez.com/api/public/v1/core/get), to your computer, then unzip. 

Next, upload to the server hosting your shopping-cart using FTP.
