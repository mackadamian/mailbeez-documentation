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

Ab Version 3.0 kann MailBeez sehr komfortabel mit dem integrierten Aktualisierungs-Programm auf die jeweils neueste Version gebracht werden.

## Updating when you get a notification

The integrated version controll will give you a notification when there is a new Version. Please click on this notification and follow the steps of the update tool.

The update tool is performing following steps
1. Check server environment
1. Download new version
1. Check if all files are writable - this ensures that you won't get a "version mix" with old, not writable files
1. Backup of /mailhive directory
1. Writing new files (all core files will be overwritten)

Returning to the MailBeez admin you should see a notification.


## Update manually

In some cases it will be necessary to open the update tool manually.

To do so please add

`?cloudloader_mode=update_core` 

to the URL of your MailBeez page, so the URL in your browser looks similar to:

`http://<shop-url>/<admin>/mailbeez.php?cloudloader_mode=update_core`

then follow the steps for updating the core system.