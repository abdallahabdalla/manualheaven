USE CASES

Purpose
Use cases answer:
"What can each actor do with the system?"

1. ACTORS
Primary Actor
Customer
Browses products
Places orders
Views confirmation

Secondary Actor
Store Owner (Simulated)
Reviews incoming orders
Updates order status (simulated system action)
For the MVP, many store-owner actions will actually be automated by JavaScript.

2. USE CASE INVENTORY
UC-01 — Browse Products
Goal
Allow customers to view available automotive apparel products.
Primary Actor
Customer
Preconditions
User has opened ManualHeaven.
Main Flow
Customer opens homepage.
System loads product catalog.
System displays products in a grid layout.
Customer reviews available products.
Success Outcome
Customer can view available products.

UC-02 — View Product Information
Goal
Allow customers to understand a product before ordering.
Primary Actor
Customer
Preconditions
Product catalog is displayed.
Main Flow
Customer views a product card.
System displays:
Product image
Product name
Product price
Customer reviews information.
Success Outcome
Customer understands product offering.

UC-03 — Place Order
Goal
Allow customer to create an order.
Primary Actor
Customer
Preconditions
Product is displayed.
Main Flow
Customer clicks "Buy Now".
System creates an order object.
System assigns status = Created.
System displays order summary.
Success Outcome
Order is successfully created.

UC-04 — Process Order
Goal
Simulate order processing.
Primary Actor
System
Preconditions
Order exists.
Main Flow
Order status begins as Created.
System changes status to Processing.
System waits predefined delay.
System changes status to Completed.
Success Outcome
Order reaches Completed status.

UC-05 — View Order Confirmation
Goal
Allow customer to confirm order completion.
Primary Actor
Customer
Preconditions
Order status = Completed.
Main Flow
System displays confirmation screen.
System shows:
Product name
Product price
Order status
Customer reviews confirmation.
Success Outcome
Customer receives confirmation.

UC-06 — Start New Order
Goal
Allow customer to begin another shopping session.
Primary Actor
Customer
Preconditions
Confirmation screen is displayed.
Main Flow
Customer clicks "Back to Store".
System returns to product catalog.
Customer may place another order.
Success Outcome
New order cycle can begin.

USE CASE RELATIONSHIPS
A simplified sequence:
Browse Products
      ↓
View Product Information
      ↓
Place Order
      ↓
Process Order
      ↓
View Confirmation
      ↓
Start New Order