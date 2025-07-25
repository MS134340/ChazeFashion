# 🛍️ ChazeFashion – Modern E-Commerce Web App

ChazeFashion is a fully responsive e-commerce web application built using **Django**, **TailwindCSS**, and **DaisyUI**. The platform enables users to browse products, manage their cart and wishlist, and complete orders with a clean, modern UI.

---

## 🚀 Features

- 🛒 Add to Cart, Remove, and Update Quantity
- ❤️ Add/Remove items from Wishlist
- 🧾 Checkout with Cart Summary
- 🔐 User Authentication (Login/Register)
- 🌐 Clean UI using TailwindCSS & DaisyUI
- 🧠 Dynamic product loading from `products.json`

---

## 📂 Project Structure

    ```bash
    ChazeFashion/
    ├── ProductCatlog/
    │   ├── __init__.py
    │   ├── settings.py
    │   ├── urls.py         <-- Main URLs
    │   └── wsgi.py
    ├── base/
    │   ├── views.py        <-- Cart, Wishlist, Auth, Orders
    │   ├── models.py
    │   ├── templates/
    │   │   ├── base.html   <-- Layout template
    │   │   ├── cart.html   <-- Cart page
    │   │   └── other templates...
    │   ├── static/
    │   │   └── css, js     <-- TailwindCSS, custom JS
    ├── data/
    │   └── products.json   <-- Sample product data
    ├── manage.py
    └── README.md
## ⚙️ Tech Stack
- Backend: Django (Python)
- Frontend: TailwindCSS, DaisyUI
- Database: SQLite (Default)
- Auth: Django's built-in authentication

## 🛠️ Setup Instructions
### 1. Clone the Repository
      ```bash
        git clone https://github.com/your-username/ChazeFashion.git
        cd ChazeFashion

### 2. Create a Virtual Environment
      ```bash
        python -m venv env
        source env/bin/activate  # Windows: env\Scripts\activate
 
### 3. Install Dependencies
      ```bash
        pip install -r requirements.txt
        
### 4. Run Migrations
      ```bash
        python manage.py migrate

 ### 5. Load Product Data (Optional)
    Ensure products.json is read in your view to populate products.

### 6. Run the Development Server
      ```bash
        python manage.py runserver
