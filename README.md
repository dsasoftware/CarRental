CarRental
=========

It is an OpenERP Module to automate the Cars Rental Process

You must add this 2 lines to the ../product/product.py file in the _columns section :

    'car_rental_id': fields.one2many('car.rental', 'product_id' , 'Product'),
  	'customer_id': fields.one2many('car.rental.contract', 'customer_id' , 'Renter Name'),
    
