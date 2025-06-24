![image](https://github.com/user-attachments/assets/a4d94f2a-77a3-4f80-baf2-20c2b9f5a5a3)# 🛒 PyCart – Terminal-Based E-Commerce Platform (Python + MongoDB)

Welcome to **PyCart**, a sleek and modern **command-line eCommerce platform** built using **Python** and **MongoDB**. Designed for developers and backend enthusiasts, PyCart simulates a real-world shopping experience — entirely in your terminal — with robust product management, user authentication, and order processing.

---

## ✨ Why PyCart?

> PyCart is more than a project — it's a **portfolio-ready backend system** that shows off your ability to:
- Interact with MongoDB using `pymongo`
- Implement real-world eCommerce logic
- Manage authentication and role-based access
- Design a CLI experience that’s functional and user-friendly

---

## 📁 Project Structure

├── cli.py # Handles user/admin interaction via terminal
├── models.py # Business logic & all database operations
├── db.py # MongoDB connection setup
├── main.py # Entry point: login/registration + flow control
└── requirements.txt # Required Python libraries


---

## 🔍 File-by-File Breakdown

models.py – Core Business Logic
This is the engine that powers PyCart.

👤 Authentication
register_user(username, password, role='user')
Adds a new user or admin.

login_user(username, password)
Verifies credentials and returns user data.

📦 Product Management
add_product(name, price, stock)
Admin-only: Adds a product to catalog.

list_products()
Returns all products.

search_product(name)
Case-insensitive product search by name.

🛒 Order System
place_order(username, product_id, quantity)
✔ Validates stock
✔ Deducts quantity
✔ Saves order with timestamp

user_orders(username)
View a user's past purchases.

🗂 Admin Reporting
get_all_orders()

get_all_users()

All operations are done securely and directly via MongoDB.

🖥️ cli.py – Command-Line User Interface
CLI menus for both Admin and User roles.

👤 User Options:
View all products (with name, price, stock)

Search products by name

Place an order

View personal order history

Stock is automatically validated, and users are informed if a product is out of stock or quantity exceeds availability.

👨‍💼 Admin Options:
Add new products to the catalog

View all users

View all orders across the platform

Robust input validation ensures clean user experience.


🚀 main.py – Application Entry Point
The main router for your app.

Handles the entire flow:

Register as user or admin

Login with role detection

If user → opens user_menu()

If admin → opens admin_menu()

![image](https://github.com/user-attachments/assets/b2bb89f8-0105-4523-84e9-7399120acbe8)
![image](https://github.com/user-attachments/assets/222ce3b6-6f4e-4f2c-a882-097f3f26cc66)
![image](https://github.com/user-attachments/assets/39260934-38cc-4197-be15-94cc410ead2a)
![image](https://github.com/user-attachments/assets/efc016b3-f5be-4a11-814f-199570422894)




