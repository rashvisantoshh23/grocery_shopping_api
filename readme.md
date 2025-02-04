# Grocery Shopping API  

This is a RESTful API for a grocery shopping application that enables users to manage accounts, browse products, add items to their cart, place orders, process payments, submit reviews, and apply discounts.  

## 📌 Features  
- **User Management**: Register, login, and manage user profiles.  
- **Product Management**: Add, update, delete, and view products.  
- **Cart Management**: Add, remove, and view items in the cart.  
- **Order Processing**: Place orders and view order history.  
- **Payments**: Process payments and retrieve payment history.  
- **Reviews & Ratings**: Submit and manage product reviews.  
- **Offers & Coupons**: Apply discounts and view available offers.  
- **Wishlist**: Save favorite items for later.  
- **General Features**: Search for products, submit feedback, and monitor API health.  

---

## 📌 API Endpoints  

### 🔹 **User Management**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/register` | Register a new user |
| `POST` | `/login` | User login |
| `GET` | `/user/{user_id}` | Retrieve user details |
| `PUT` | `/user/{user_id}` | Update user details |
| `DELETE` | `/user/{user_id}` | Delete user account |

### 🔹 **Product Management**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/products` | Add a new product |
| `GET` | `/products/{product_id}` | Get product details |
| `PUT` | `/products/{product_id}` | Update product details |
| `DELETE` | `/products/{product_id}` | Remove a product |
| `GET` | `/products` | Retrieve all products |

### 🔹 **Cart Management**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/cart/{user_id}` | View cart items |
| `POST` | `/cart/{user_id}/add` | Add an item to the cart |
| `POST` | `/cart/{user_id}/remove` | Remove an item from the cart |
| `POST` | `/cart/{user_id}/clear` | Clear the cart |

### 🔹 **Order Processing**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/orders/{user_id}` | Place an order |
| `GET` | `/orders/{order_id}` | Get order details |
| `DELETE` | `/orders/{order_id}` | Cancel an order |
| `GET` | `/orders/{user_id}/history` | View order history |

### 🔹 **Payment Management**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/payments/{user_id}` | Process a payment |
| `GET` | `/payments/{user_id}/history` | Retrieve payment history |

### 🔹 **Reviews & Ratings**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/products/{product_id}/review` | Add a review |
| `GET` | `/products/{product_id}/reviews` | Get all reviews |
| `DELETE` | `/products/{product_id}/review/{review_id}` | Delete a review |

### 🔹 **Offers & Coupons**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/offers` | Get available offers |
| `POST` | `/apply-coupon` | Apply a discount coupon |

### 🔹 **Wishlist Management**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/wishlist/{user_id}` | View wishlist items |
| `POST` | `/wishlist/{user_id}/add` | Add an item to the wishlist |
| `POST` | `/wishlist/{user_id}/remove` | Remove an item from the wishlist |

### 🔹 **General APIs**  
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/search` | Search for products |
| `POST` | `/feedback` | Submit user feedback |
| `GET` | `/app-stats` | Retrieve app statistics |
| `GET` | `/health-check` | Check API server health |

---

## 🚀 Getting Started  

### **🔧 Prerequisites**  
Ensure you have Python and Flask installed:  

```bash
pip install flask
