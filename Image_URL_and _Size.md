## Documentation for Product Detail, Image URL and Size
### Image sizes: 

We have to provide a product ID   in URL(http://site-URL/image_api/product.php?id=123..). 

It will also get the ID, Name and price of product as well. 

From product ID it will get the attachment ID. 

Through attachment ID it will get image for that product and make it’s sizes. 

This detail should be in array format and as well as in JSON format also. 

Sizes will thumbnail, large, medium,  woocommerce_single,  medium_large etc. 

URL should be like this “file_name-size_name.ext”. (e.g) abc-thumbnail.jpg. 

#### Sizes width would be about: 

thumbnail                  :  150px 

medium                          : 300px 

medium_large               : 768px 

large                                : 1024px 

woocommerce_single  : 600px 

#### How to access ? 

This is an example link here: 
http://foodu.ctsdemo.com/image_api/product.php?id=5172

#### NOTE: 
New images which are uploaded will be converted in different sizes old are not.
