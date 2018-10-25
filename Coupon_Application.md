## Documentation for Coupon Application
### Coupon discount types:
There are three types of coupon discount
   #### Percentage discount.
   #### Fixed cart discount.  
   #### Fixed product discount.  
     
    1) A Percentage discount -A Percentage discount for selected products only. For example, if the cart contains three (3) items @ $20 each = $60, a coupon for 10% off applies a discount of $6. 

     2) Fixed cart discount – A fixed total discount for the entire cart. For example, if the cart contains three (3) items @ $20 each = $60, a coupon for $10 off gives a discount of $10. 

     3) Fixed product discount – A fixed total discount for selected products only. Customer receives a set amount of discount per item. For example, three (3) items @ $20 each with a coupon for $10 off applies a discount of $30. 
 ### Scenario to Apply a coupon by user:    
       When a user enters a coupon code with its order first its validity checked. If that coupon exists then it will be applying on that order 

      Now we have to send that coupon code with our order in JSON format with its name and key. 

      We have modified our JSON and set a scenario for send a coupon which is working. 

      Coupon in JSON: 

      “key”: “name”  e.g 

      "coupon_code":"XXX" 
      
      order JSON would be like this
   
      "line_items": [
    {
      "product_id": XXX,
      "quantity": XX,
      "meta_data" :[
       {
        "key" : "delivery_time",
        "value" : "XXX"
       },
       {
        "key" : "cost_price",
        "value" : "XXX"
       }
       ]
     }
    ],
       "shipping_lines" :[
    {
      "method_id" : "flat_rate",
      "method_title" : "Flat Rate",
      "total": "XXX"
    }
     ]
