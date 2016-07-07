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


### API Calls


GET `http://<myshop.com>/mailhive.php/api/private/v1.0/product/reviews/`

#### Mandatory Parameters

| Parameter    	| Type 	| Description                            	|
|--------------	|------	|----------------------------------------	|
| apikey       	| text 	| Your personal API-Key                  	|
| products_id  	| int  	| Products-Id of Product to show reviews 	|


#### Optional Parameters


| Parameter    	| Type 	| Description                            	|
|--------------	|------	|----------------------------------------	|
| languages_id 	| int  	| limit reviews to this language_id        	|
| count        	| int  	| Number of reviews to show              	|
| rating_min   	| int  	| minimum number of stars a rating must have to be shown e.g. 4            	|
| template     	| text 	| the name of the custom template, e.g. mytemplate will look for the file mytemplate.tpl.html              	|



####Return

Html-Output of the product reviews formatted using the configured template

####Example

```
http://<myshop.com>/mailhive.php/api/private/v1.0/product/reviews/?products_id=21&languages_id=0&count=2&rating_min=4&template=html.tpl.html&apikey=123
```


### API Client Library

To use the Product Reviews API please copy the API client files as you can find them on your MailBeez Server:

```
/mailhive/configbeez/config_api_product/apibeez/api_private_product_reviews/_client
```


to the server where you want to integrate the product reviews into. This could be a blog-page around specific products.

Edit the file `config.php`

```
define('MAILBEEZ_API_ENTRYPOINT', 'http://<myshop.com>/mailhive.php/api/');
define('MAILBEEZ_API_KEY', '<your api key>');
```

with the matching settings.

Then you can use the API client as following on any PHP file
```
include_once('mailbeez_productreviews_client.php');
$reviewsObj = new mailbeez_productreviews_client();
$reviewsOutput = $reviewsObj->showReviews(array('products_id' => 112, 'languages_id' => null, 'count' => 3, 'rating_min' => 4, 'template' => 'productreviews' ));
echo  $reviewsOutput['result'];
```
to include product reviews for - in this case - product with `products_id=112`.


The html is generated using the smarty templates located in:
```bash
/mailhive/configbeez/config_api_product/apibeez/api_private_product_reviews/templates/
```
 

The default template `default_productreviews.tpl.html` will be overwritten with updates, so you should not edit it.

For customization make a copy of this template and rename it to e.g. `productreviews.tpl.html` and apply your customization.

The API-Call
```
$reviewsOutput = $reviewsObj->showReviews(array('products_id' => 112, 'languages_id' => null, 'count' => 3, 'rating_min' => 4, 'template' => 'productreviews' ));
```
contains the parameters as listed above you can use to controll the output.
