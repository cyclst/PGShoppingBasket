Shopping Basket Discount Task

The company issues two types of voucher for customers to gain discounts on shopping baskets. 
Gift Voucher:
 - Can be redeemed against the value of a basket. 
 - Multiple gift vouchers can be applied to a basket. 

Offer vouchers:
 -  Have a threshold that needs to be matched or exceeded before a discount can be applied e.g. £5.00 off of  baskets totalling £50
 - Only a single offer voucher can be applied to a basket. 
 - Maybe applicable to only a subset of products.

Offer and Gift vouchers can be used in conjunction. If a customer applies an offer voucher to a basket that will not satisfy the threshold or a customer removes item/changes an items quantity resulting in a voucher not being a message will need to be displayed to the customer.  
Gift vouchers can only be redeemed against non gift voucher products and purchase of gift vouchers do no contribute to discountable basket total.
Write an application that represents a basket and has the ability to handle the following scenarios:

(You need not create a UI for this application).

Basket 1:
1 Hat @ £10.50
1 Jumper @ £54.65
\------------
1 x £5.00 Gift Voucher XXX-XXX applied
\------------
Total: £60.15

Basket 2:
1 Hat @ £25.00
1 Jumper @ £26.00
\------------
1 x £5.00 off Head Gear in baskets over £50.00 Offer Voucher YYY-YYY applied
\------------
Total: £51.00
Message: “There are no products in your basket applicable to voucher Voucher YYY-YYY .”

Basket 3:
1 Hat @ £25.00
1 Jumper @ £26.00
1 Head Light (Head Gear Category of Product)  @ £3.50
\------------
1 x £5.00 off Head Gear in baskets over £50.00 Offer Voucher YYY-YYY applied
\------------
Total: £51.00

Basket 4:
1 Hat @ £25.00
1 Jumper @ £26.00
\------------
1 x £5.00 Gift Voucher XXX-XXX applied
1 x £5.00 off baskets over £50.00 Offer Voucher YYY-YYY applied
\------------
Total: £41.00

Basket 5:
1 Hat @ £25.00
1 £30 Gift Voucher @ £30.00
\------------
1 x £5.00 off baskets over £50.00 Offer Voucher YYY-YYY applied
\------------
Total: £55.00
\------------
Message: “You have not reached the spend threshold for voucher YYY-YYY. Spend another £25.01 to receive £5.00 discount from your basket total.”


Nouns:
 - Shopping Basket
   - Total
   - Item
     - Quantity
   - Discount
   - Message
 - Gift Voucher
   - Amount
 - Offer Voucher
   - Amount
   - [Qualifying] Product Categories
   - Shopping Basket Threshold
 - Customer
 - Product
   - Is a Gift Voucher
   - Amount
 - Product Category

Verbs:
 - Customer puts products in Shopping Basket
 - Customer applies a Voucher to Shopping Basket
 - Customer sees Shopping Basket Total
 - Customer changes Quantity of Products in Shopping Basket
 - Shopping Basket satifies Offer Voucher Threshold
 - Message displayed to Customer
 - Total excludes Gift Voucher Amount

