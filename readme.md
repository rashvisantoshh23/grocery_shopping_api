# Grocery Shopping API

This is a REST API for a grocery shopping application that allows users to manage accounts, browse products, add items to carts, place orders, process payments, submit reviews, and apply discounts.

## Features
- **User Management**: Register, login, and manage user profiles.
- **Product Management**: Add, update, delete, and view products.
- **Cart Management**: Add, remove, and view items in the cart.
- **Order Processing**: Place orders and view order history.
- **Payments**: Process payments and retrieve payment history.
- **Reviews & Ratings**: Submit and manage product reviews.
- **Offers & Coupons**: Apply discounts and view available offers.
- **Wishlist**: Save favorite items.
- **General Features**: Search products, submit feedback, and monitor API health.

## API Endpoints

### User Management
- **POST /register** - Register a new user
- **POST /login** - Login a user
- **GET /user/{user_id}** - Retrieve user details
- **PUT /user/{user_id}** - Update user details
- **DELETE /user/{user_id}** - Delete user account

### Product Management
- **POST /products** - Add a new product
- **GET /products/{product_id}** - Get product details
- **PUT /products/{product_id}** - Update product details
- **DELETE /products/{product_id}** - Remove a product
- **GET /products** - Retrieve all products

### Cart Management
- **GET /cart/{user_id}** - View cart items
- **POST /cart/{user_id}/add** - Add item to cart
- **POST /cart/{user_id}/remove** - Remove item from cart
- **POST /cart/{user_id}/clear** - Clear the cart

### Order Processing
- **POST /orders/{user_id}** - Place an order
- **GET /orders/{order_id}** - Get order details
- **DELETE /orders/{order_id}** - Cancel an order
- **GET /orders/{user_id}/history** - View order history

### Payment Management
- **POST /payments/{user_id}** - Process a payment
- **GET /payments/{user_id}/history** - Retrieve payment history

### Reviews & Ratings
- **POST /products/{product_id}/review** - Add a review
- **GET /products/{product_id}/reviews** - Get all reviews
- **DELETE /products/{product_id}/review/{review_id}** - Delete a review

### Offers & Coupons
- **GET /offers** - Get available offers
- **POST /apply-coupon** - Apply a discount coupon

### Wishlist Management
- **GET /wishlist/{user_id}** - View wishlist items
- **POST /wishlist/{user_id}/add** - Add item to wishlist
- **POST /wishlist/{user_id}/remove** - Remove item from wishlist

### General APIs
- **GET /search** - Search for products
- **POST /feedback** - Submit feedback
- **GET /app-stats** - Retrieve app statistics
- **GET /health-check** - Check API server health


