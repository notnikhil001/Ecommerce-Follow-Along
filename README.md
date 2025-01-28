# Ecommerce-Follow-Along

1. REST API
A REST API (Representational State Transfer Application Programming Interface) allows communication between a client (frontend) and a server (backend) using HTTP methods like GET, POST, PUT, DELETE.
In a MERN stack:

Backend: Built using Node.js and Express.js to handle API endpoints.
Frontend: The React.js app sends requests to these APIs to fetch or send data.
Database: MongoDB stores the data retrieved or updated via APIs.

2. MERN Stack
The MERN stack is a full-stack development framework comprising:

MongoDB: NoSQL database for storing data in JSON-like documents.
Express.js: Backend web framework for building APIs and handling server logic.
React.js: Frontend library for building user interfaces.
Node.js: JavaScript runtime for executing server-side code.
This stack enables JavaScript to be used across the entire application.

3. Order Handling
Order handling involves managing customer orders through the app.
Key functionalities:

Placing Orders: API to accept user order details (product, quantity, payment status, etc.).
Order Tracking: API to fetch order status and history.
Admin Features: APIs for order confirmation, shipment, or cancellation.
Database: MongoDB stores order-related data.

4. Product Listing and Management
This involves creating, reading, updating, and deleting (CRUD) products.
Key functionalities:

Product Listing: API to fetch all available products for display on the frontend.
Product Details: API to show details of a specific product.
Admin Management:
Add new products.
Update product details (price, stock, description).
Delete products.
Database: MongoDB stores product data.

5. User Authentication
This ensures only authorized users can access or modify resources.
Key functionalities:

Signup: API to create a new user account.
Login: API to verify user credentials and issue a JSON Web Token (JWT).
Authentication Middleware: Verifies the JWT for protected routes.
Roles:
User: Access to general features like browsing and ordering.
Admin: Access to product and order management.
Firebase Auth: Optionally used for managing authentication in MERN apps.
