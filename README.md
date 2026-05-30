# 👟 Shoe Store

A static shoe store built with React, featuring a shopping cart and checkout flow. This project was built to practice React state management with Redux Toolkit and component-driven UI development using Tailwind CSS.

---

## ✨ Features

- 🛍️ **Product Listings** — Hero section and sales sections showcasing popular & top-rated shoes
- 🛒 **Shopping Cart** — Add/remove items, view quantity and total price
- 🔔 **Toast Notifications** — Real-time feedback on cart actions via `react-hot-toast`
- 📱 **Responsive Design** — Mobile-friendly layout with Tailwind CSS
- 🔗 **Smooth Navigation** — Navbar with cart toggle and social links in footer

---

## 🛠️ Tech Stack

| Layer         | Technology                          |
|---------------|-------------------------------------|
| Framework     | React 18 + Vite                     |
| State Mgmt    | Redux Toolkit + React-Redux         |
| Routing       | React Router DOM v6                 |
| Styling       | Tailwind CSS v3                     |
| Icons         | Heroicons (React)                   |
| Notifications | react-hot-toast                     |
| Bundler       | Vite                                |

---

## 📁 Project Structure

```
shoe-store/
├── public/
│   └── shoes.png               # Public static asset
├── src/
│   ├── app/
│   │   ├── CartSlice.js        # Redux slice for cart state (add, remove, increment, decrement)
│   │   └── Store.js            # Redux store configuration
│   ├── assets/                 # All images & SVG icons (products, logo, social icons, etc.)
│   ├── components/
│   │   ├── Cart/
│   │   │   ├── CartCount.jsx   # Displays total item count and price summary
│   │   │   ├── CartEmpty.jsx   # Empty cart placeholder UI
│   │   │   └── CartItem.jsx    # Individual cart item with qty controls
│   │   ├── utils/
│   │   │   ├── Item.jsx        # Reusable product card (image, name, price, add-to-cart)
│   │   │   ├── SocialLink.jsx  # Reusable social media icon link
│   │   │   └── Title.jsx       # Reusable section title component
│   │   ├── Cart.jsx            # Cart sidebar/overlay component
│   │   ├── Footer.jsx          # Footer with links and social icons
│   │   ├── Hero.jsx            # Hero/banner section
│   │   ├── Navbar.jsx          # Top navigation bar with cart toggle
│   │   ├── Sales.jsx           # Sales section (popular & top-rated)
│   │   └── index.js            # Barrel export for all components
│   ├── data/
│   │   └── data.js             # Static product data (hero, popular sales, top-rated sales)
│   ├── App.jsx                 # Root component — composes all sections
│   ├── App.css                 # App-level styles
│   ├── index.css               # Global styles & Tailwind directives
│   └── main.jsx                # Entry point — mounts app with Redux Provider
├── index.html                  # HTML shell
├── vite.config.js              # Vite configuration
├── tailwind.config.js          # Tailwind CSS configuration
├── postcss.config.js           # PostCSS configuration
└── package.json                # Dependencies and scripts
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js ≥ 16
- npm

### Installation

```bash
# Clone the repository
git clone https://github.com/me-bipin99/shoe-store.git
cd shoe-store

# Install dependencies
npm install

# Start development server
npm run dev
```

The app will be available at `http://localhost:5173`.

### Available Scripts

| Command         | Description                        |
|-----------------|------------------------------------|
| `npm run dev`   | Start local development server     |
| `npm run build` | Build for production               |
| `npm run preview` | Preview production build locally |
| `npm run lint`  | Run ESLint checks                  |

---

## 📦 State Management

Cart state is managed globally with **Redux Toolkit**:

- `addToCart` — adds a product to the cart
- `removeFromCart` — removes a product from the cart
- `incrementQuantity` / `decrementQuantity` — adjusts item quantity

---

> ⚠️ This is a **static demo project** — no backend or real payment processing is included.
