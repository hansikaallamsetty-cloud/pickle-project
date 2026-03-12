# 🥒 Homemade Pickles & Snacks — Taste the Best

A full-featured Flask e-commerce application with authentication, cart, checkout, inventory management, subscriptions, and personalized recommendations. Designed for local development with a clear path to AWS DynamoDB + EC2 deployment.

---

## 📁 Project Structure

```
project/
├── app.py                    # Main Flask application (routes, data, logic)
├── requirements.txt
├── templates/
│   ├── base.html             # Shared layout (navbar, footer, flash messages)
│   ├── index.html            # Home page with hero, featured products, subscriptions
│   ├── products.html         # Product catalog with category filters
│   ├── product_detail.html   # Single product view with quantity selector
│   ├── login.html            # User login
│   ├── register.html         # User registration
│   ├── cart.html             # Cart with recommendations
│   ├── checkout.html         # Checkout with simulated payment
│   └── order_success.html    # Order confirmation
└── static/
    ├── css/
    │   └── styles.css        # Full dark theme design system
    └── images/               # Product placeholder images (PNG)
```

---

## 🚀 Quick Start

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Run the app

```bash
python app.py
```

### 3. Open in browser

```
http://localhost:5000
```

---

## ✅ Features

| Feature                    | Status |
|---------------------------|--------|
| Product catalog (12 items) | ✅ |
| Category filters           | ✅ |
| User registration & login  | ✅ |
| Session-based cart         | ✅ |
| Add / remove / update cart | ✅ |
| Checkout simulation        | ✅ |
| Inventory deduction        | ✅ |
| Order confirmation         | ✅ |
| Personalized recommendations| ✅ |
| Subscription plans         | ✅ |
| Responsive dark UI         | ✅ |

---

## ☁️ AWS Integration Plan

| Component | Current            | AWS Target         |
|-----------|--------------------|--------------------|
| Users     | Python dict (RAM)  | DynamoDB `Users`   |
| Products  | Python dict (RAM)  | DynamoDB `Products`|
| Orders    | Python dict (RAM)  | DynamoDB `Orders`  |
| Subscriptions | Python dict  | DynamoDB `Subscriptions` |
| Images    | `static/images/`   | S3 Bucket          |
| Server    | `flask run`        | EC2 + Gunicorn + Nginx |
| Sessions  | Flask session      | ElastiCache (Redis)|

---

## 🎨 Design

- **Font:** Poppins + Playfair Display (Google Fonts)
- **Colors:** Black `#000000` · Yankees Blue `#14213D` · Dark Orange `#FCA311` · Platinum `#E5E5E5`
- **Theme:** Dark, modern e-commerce with animated hero and floating jar visuals
<<<<<<< HEAD
=======
# pickle-project
>>>>>>> 99f5c9e759de077603f5e308578d7c036ea61c13
