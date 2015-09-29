---
title: 'Products API'
template: docs
taxonomy:
    category: [docs]
    tag: [pro]
    
---
This API Module groups product related API calls.


##Product Reviews API

The Product Reviews API allows you to display your product reviews on any PHP based page on any other server.

To use the Product Reviews API please copy the API client files as your find them on your MailBeez Server:

```
/mailhive/configbeez/config_api_product/apibeez/api_private_product_reviews/_client
```


to the server where you want to integrate the product reviews.

Edit the file `config.php`

```
define('MAILBEEZ_API_ENTRYPOINT', 'http://<myblog.com>/mailhive.php/api/');
define('MAILBEEZ_API_KEY', '<your api key>');
```

with the matching settings.

Then you can use the API client as following
```
include_once('mailbeez_productreviews_client.php');
$reviewsObj = new mailbeez_productreviews_client();
$reviewsOutput = $reviewsObj->showReviews(array('products_id' => 112, 'languages_id' => null, 'count' => 3, 'rating_min' => 4, 'template' => 'productreviews' ));
echo  $reviewsOutput['result'];
```
to include product reviews for - in this case - product with `products_id=112`.




The html is generated using the smarty templates located in:
```
/mailhive/configbeez/config_api_product/apibeez/api_private_product_reviews/templates/
```
 

The default template `default_productreviews.tpl.html` will be overwritten with updates, so you should not edit it.

For customization make a copy of this template and rename it to e.g.

`productreviews.tpl.html`

and apply your customization.

The API-Call
```
$reviewsOutput = $reviewsObj->showReviews(array('products_id' => 112, 'languages_id' => null, 'count' => 3, 'rating_min' => 4, 'template' => 'productreviews' ));
```
contains following parameters you can use to controll the output:

**products_id**: The Id of the product

**languages_id**: limit reviews to this language_id

**count**: number of reviews to display

**rating_min**: minimun number of stars a rating must have to be shown

**template**: the name of the custom template, e.g. `mytemplate` will look for the file `mytemplate.tpl.html`

