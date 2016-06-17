---
# http://learn.getgrav.org/content/headers
title: '[ZenCart] Paket Tracking' 
slug: filter_add_pakettracking_zencart
published: true
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
    tag: [pro]
# added collection selector
module:
    code: 'filter_add_pakettracking_zencart'
    category: [filterbeez]
    compatiblity: [comp_zencart]
    pro: 'pro'
    cert: 'true' 
author:
    name: admin
metadata:
    author: admin

---

Dieses Modul ergänzt die [Erweiterung für Zencart: Paket Tracking ](https://www.zen-cart-pro.at/forum/vbdownloads.php?do=download&downloadid=181) und erlaubt, die Tracking-Informatione komfortabel in jede Bestell-relatierte MailBeez Email z.B. [Status-Änderungs-Benachrichtigung](/dokumentation/mailbeez/notification_order_status) einzufügen.


Es werden alle Daten-Felder der Erweiterung zur Verfügung gestellt:


``` 
[[$data.order.paket_tracking.track_id1]] // track_id1
[[$data.order.paket_tracking.track_id2]] // track_id2
[[$data.order.paket_tracking.track_id3]] // track_id3
[[$data.order.paket_tracking.track_id4]] // track_id4
[[$data.order.paket_tracking.track_id5]] // track_id5
[[$data.order.paket_tracking.track_id6]] // track_id6
[[$data.order.paket_tracking.track_day]] // track_day
[[$data.order.paket_tracking.track_month]] // track_month
[[$data.order.paket_tracking.track_year]] // track_year
``` 

Und mit etwas Smarty-Logik können die Links zu den Tracking-System der verschiedenen Carrier zusammengestellt werden.

**Beispiel:**

```
[[if $data.order.paket_tracking.track_id1 ]]
    <a href="http://carrier1.com?track=[[$data.order.paket_tracking.track_id1]]"> Tracking Link Carrier 1 </a>
[[elseif $data.order.paket_tracking.track_day]]
    <a href="http://carrier2.com?track=[[$data.order.paket_tracking.track_id2]]&day=[[$data.order.paket_tracking.track_day]]"> Tracking Link Carrier 2 </a>
[[/if]]
``` 

