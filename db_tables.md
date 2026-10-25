# Database Table Designs

Table Description

## Users
Stores customer and administrator accounts
 




| user_id | Unique identifier for each user |

| username | unique name for each user |

| password_hash | Integrity for each password |

| first_name | First name of a user |

| last_name | Last name of a user |

| email | Email address of the user |

| address | Delivery and Billing address of the user |

| role | Permissions assigned to user |

## Products Table

Stores all of the products offered in DuckMart.
 

| product_id | Unique Identifier for each product |

| name | Name product is listed as |

| image | link to image of product |

| category | Group such as "bakery", "deli", etc. |

| price | selling price |

| stock | Number of items in stock |

| on_sale | Yes or No value. If yes, product will be displayed at a discount and shown in the 'Deals' section of website |

## Categories

Organizes products by grocery category.


| category_id | Unique Identifier for category |

| category_name | Name category is listed as |

## Shopping_Carts

Tracks customers' shopping carts.

| cart_id | Unique Identifier for each cart |

| user_id | Unique Identifier for each user |

| session_id | Unique Identifier that links user to cart |

## Cart_Items

Tracks the products and quantities in each cart. 

| cart_item_id | Unique Identifier for item in the cart |

| cart_id | Unique Identifier for the cart |

| cart_item_id | Unique Identifier for item in the cart |

| product_id | Unique Identifier for each product |

| quantity | Number of each item in cart |

## Orders

Stores customer orders and their delivery information.

| order_id | Unique Identifier for each order the user makes |

| user_id | Unique Identifier for each user |

| order_date | Tracks the date the the order was made |

| delivery_slot_id | Unique Identifier for the delivery priority |

| status | The status of the order(delivered, shipped, failed delivery, etc.)

## Order_Items

Stores the induvidual products in each order. 

| order_item_id | Unique Identifier for item in the order |

| order_id | Unique Identifier for each order |

| product_id | Unique Identifier for each product |

| quantity | Number if items in each order |

| unit_price | Price of one individual product in the order |

## Delivery_Slots
Stores available delivery times.

| delivery_slot_id | Unique Identifier for the delivery priority |

| delivery_date | Estimated date the products will be delivered |

| start_time | Start of the delivery window |

| end_time | End of the delivery window |





















