Click to Run starts the workflow when you press Execute.
Warehouse Setup creates 4 warehouses (Delhi, Mumbai, Bengaluru, Kolkata) with their stock and product weights.
Sample Orders creates 15 sample customer orders.
Validate Orders removes duplicate orders and rejects any order with no valid items. This leaves 14 orders, 1 of them rejected.
Fraud Check gives each order a fraud score. It looks at new accounts, very high order value, cash on delivery, night-time orders, bulk quantities and repeat orders. The score marks each order as Clear, Review or Block.
Hold Order? splits the orders into two groups.
Blocked and rejected orders go to Fraud Hold Queue, which lists the reason and the action to take.
All other orders carry on to the next step.
Apply Pricing applies the coupon, the loyalty tier discount and 18% GST. It also rejects invalid coupons.
Prioritize Orders puts express orders first, then higher loyalty tiers.
Allocate Inventory takes stock from the nearest warehouse. If that warehouse runs short, it takes the rest from the next nearest, and anything left over becomes a backorder.
Shipping Plan works out the shipments, the shipping cost by weight and distance, and the delivery time. Gold and Platinum customers ship free.
Fully Fulfilled? splits the orders again.
Complete orders go to Ready To Ship, which creates tracking IDs.
Orders with missing stock go to Backorder Handling, which sets a 7-day restock time and a compensation offer.
Customer Messages writes a message for each customer: confirmed, under review, or partly shipped.
Warehouse Utilization shows how much stock each warehouse used and flags low stock.
Business Dashboard adds up revenue, average order value, fraud results, fulfillment rate and top products.
Final Report puts everything into one report, in the report field.
Final Output adds a “completed successfully” status.
