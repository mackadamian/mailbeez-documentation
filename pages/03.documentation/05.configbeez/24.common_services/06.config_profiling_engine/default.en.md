---
title: Profiling engine
slug: config_profiling_engine
routes:
    default: /documentation/configbeez/config_profiling_engine
        
published: true
template: docs
visible: true
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    migration_status: done
    category: [docs]
    tag: [pro]
module:
    code: 'pro'
    category: [pro]
    compatiblity: [comp_osc,comp_cre,comp_digi,comp_zencart,comp_xtc,comp_gambio]   
    pro: 'pro'

# added collection selector

author:
    name: admin
metadata:
    author: admin

---

Under construction - the MailBeez profiling engine allows you to tag customers and orders based on rules. 

These tags can be utilized by other controll-modules to controll the behaviour and content of Email modules


Examples

- Tag all customer, who never purchase product B with tag "upsell-B"
- Tag all customer, who only purchase from category X with tag "only-cat-X"
- Tag all orders containing product H with "product-H"



Modules utilizing the tags are:

- [Profile Filter](/documentation/filterbeez/filter_check_profile)  
 Examples
      - only send a Birthday coupon to customers tagged with "upsell-B"
      - never send a product review reminder after orders containing "product H"
    
    

- [Profile Content](/documentation/filterbeez/filter_add_profiling_content)  
 Examples
      - insert upsell content partial promoting product B to all emails for customers tagged with "upsell-B"



- [Profile Information](/documentation/filterbeez/filter_add_profiling)  
 Examples
      - build some custom logic code using order and/or customer profiling


