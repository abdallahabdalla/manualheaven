TO-BE PROCESS

Step 1: Customer Enters Store
User opens the ManualHeaven homepage.
System behavior:
Displays header (ManualHeaven branding)
Shows centered info bar (simulation notice)
Loads product grid

Step 2: Browse Products
Customer views automotive apparel catalog.
System behavior:
Products are rendered from a static JS array
Each product card shows:
Product name
Price
Image placeholder
“Buy Now” button
Key difference from AS-IS:
No product detail pages (simplified UX)

🛒 Step 3: Product Selection (Simulated Order)
Customer clicks “Buy Now”.
System behavior:
System creates a temporary “order object” in JavaScript
Example:
Order {
 productName: "Racing Hoodie",
 price: 49.99,
 status: "Created"
}
UI immediately transitions to “Order Summary view”

Step 4: Order Processing (Simulation Engine)
Instead of real backend processing:
System simulates lifecycle:
Created → Processing → Completed
Behavior:
After clicking order:
Status shows “Processing…”
After short delay (e.g., setTimeout in JS):
Status changes to “Completed”

Step 5: Order Completion Screen
User sees confirmation screen.
System displays:
Product name
Price
Order status: Completed
Simple confirmation message:
“Your order has been successfully processed”

Step 6: Reset or New Order
User can:
Return to homepage
Place another simulated order
No cart persistence required in MVP.
