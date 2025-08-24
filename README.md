
# 🚗 BMW Cars E-commerce Store

An interactive **BMW e-commerce web application** that allows users to browse BMW car models, add them to a cart, and checkout with customer details and payment options. The backend is built with **Node.js & Express**, while the frontend uses **HTML, CSS, and JavaScript**.

---

## 📂 Project Structure

```
├── index.html       # Main frontend page (Home, Products, Cart, Checkout)
├── styles.css       # Styling for the frontend
├── script.js        # Frontend logic (cart, checkout, payment handling)
├── server.js        # Express backend server
├── order.js         # Example order data (JSON format)
├── package.json     # Node.js project configuration and dependencies
```

---

## ✨ Features

* **Home Page** with featured BMW models.
* **Product Listing** with car details and "Add to Cart" functionality.
* **Shopping Cart** to review selected cars and total price.
* **Checkout Form** with:

  * Customer details (name, email, phone, address)
  * Multiple payment methods (Credit Card, PayPal, Bank Transfer)
* **Credit Card Validation Section** (visible only if selected).
* **Backend Order Handling** with Express.js:

  * Saves customer orders into `orders.json`.
  * Provides a `/checkout` API for order submission.
* **Responsive Design** for desktop and mobile users.

---

## 🛠️ Tech Stack

* **Frontend**: HTML, CSS, Vanilla JavaScript
* **Backend**: Node.js, Express.js
* **Data Storage**: JSON file (`orders.json`)
* **Dependencies**:

  * `express` – Web framework for Node.js
  * `cors` – Enable cross-origin requests

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/bmw-cars-store.git
cd bmw-cars-store
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Run the Server

```bash
npm start
```

Server will start at: **[http://localhost:3000](http://localhost:3000)**

### 4️⃣ Open Frontend

Simply open `index.html` in a browser.
The frontend will interact with the backend for checkout requests.

---

## 📡 API Endpoints

### `GET /health`

Check if the server is running.
**Response:**

```json
"Server is running"
```

### `POST /checkout`

Submit an order.
**Request Body Example:**

```json
{
  "customer": {
    "name": "John Doe",
    "email": "john@example.com",
    "phone": "555-123-4567",
    "address": "123 Auto Lane"
  },
  "paymentMethod": "credit",
  "paymentDetails": {
    "cardNumber": "1234 5678 9012 3456",
    "cardExpiry": "12/25",
    "cardCvc": "123"
  },
  "cart": [
    { "id": 1, "name": "BMW M3", "price": 70000 },
    { "id": 2, "name": "BMW X5", "price": 60000 }
  ],
  "total": 130000,
  "timestamp": "2025-04-19T12:00:00.000Z"
}
```

**Response:**

```json
{ "message": "Order received" }
```

---

## 🎨 Screenshots

* **Home Page with Featured Cars**
* **Products Listing**
* **Cart & Checkout Form**

*(You can add screenshots here for better visualization.)*

---

## 📌 Future Enhancements

* ✅ Database integration (MongoDB/MySQL) instead of JSON file.
* ✅ User authentication (login & signup).
* ✅ Admin panel to manage orders and inventory.
* ✅ Payment gateway integration (Stripe/PayPal API).

---

## 👨‍💻 Author

Developed as a **BMW Cars Store E-commerce Project** using web technologies.

---

