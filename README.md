# 🍪 The Nutty Choco Morsels (TNCM) Web Application

Welcome to the official repository for **The Nutty Choco Morsels (TNCM)** web application. This is a Progressive Web App (PWA) designed for ordering delicious bakery items, tracking orders, and managing deliveries.

## 🚀 Features

*   **Online Ordering System:** Browse the menu, add items to the cart, and place orders seamlessly.
*   **User Authentication:** Secure login and registration using Firebase Auth (Google Sign-In & Email/Password).
*   **Real-time Order Tracking:** innovative scooter animation and step-by-step updates for order status.
*   **Delivery Management:**
    *   **Home Delivery:** Integrated map selection and address management.
    *   **Self Pickup:** Option to pick up orders directly from the store.
*   **Terms & Conditions:** Mandatory acknowledgment that orders cannot be cancelled after confirmation.
*   **PWA Support:** Installable on mobile and desktop for a native-like experience.
*   **Admin Features (Backend):** Order management via Firebase Console.

## 🛠️ Technology Stack

*   **Frontend:** HTML5, CSS3, Vanilla JavaScript
*   **Backend / Database:** Firebase Firestore
*   **Authentication:** Firebase Authentication
*   **Hosting:** Vercel / Firebase Hosting
*   **Maps:** Leaflet / OpenStreetMap (Nominatim API for Geocoding)

## 📂 Project Structure

```
TNCM-Web-Application/
├── CSS/                  # Stylesheets for the application
│   └── style.css
├── JS/                   # JavaScript logic files
│   ├── script.js         # Main application logic
│   ├── modal-injector.js # Handles modal UI injections (Cart, Profile, T&C)
│   ├── delivery-map.js   # Map integration logic
│   ├── bill.js           # Bill generation logic
│   └── firebase-config.js# Firebase configuration (not tracked)
├── Pages/                # Additional HTML pages
│   ├── about.html
│   ├── contact.html
│   └── tracking.html
├── assets/               # Images and icons
├── index.html            # Main entry point (Home/Menu)
├── sw.js                 # Service Worker for PWA features
├── manifest.json         # Web App Manifest
└── vercel.json           # Vercel deployment configuration
```

## ⚙️ Setup & Installation

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/your-username/TNCM-web.git
    cd TNCM-web
    ```

2.  **Configure Firebase:**
    *   Create a `JS/firebase-config.js` file (if not present) with your Firebase credentials:
    ```javascript
    const firebaseConfig = {
        apiKey: "YOUR_API_KEY",
        authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
        projectId: "YOUR_PROJECT_ID",
        storageBucket: "YOUR_PROJECT_ID.appspot.com",
        messagingSenderId: "YOUR_SENDER_ID",
        appId: "YOUR_APP_ID"
    };
    ```

3.  **Run Locally:**
    *   You can use **Live Server** (VS Code Extension) or any simple HTTP server.
    *   Example using Python:
        ```bash
        python -m http.server 8000
        ```
    *   Open `http://localhost:8000` in your browser.

## 📝 Recent Updates

*   **Terms & Conditions:** Added a mandatory checkbox in the checkout flow. Users must acknowledge that *orders cannot be cancelled after confirmation* before placing an order.
*   **Order Validation:** Enhanced `placeOrder` logic to strictly enforce T&C acceptance.

## 🤝 Contribution

Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

---
*Created with ❤️ for The Nutty Choco Morsels*
# for-change
