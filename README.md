# Tech Heaven - E-Commerce Platform 📱

> **Your One-Stop Destination for Quality Smartphones** - Modern E-Commerce Solution with Complete Product Management

[![React](https://img.shields.io/badge/React-18.2.0-blue?style=flat-square&logo=react)](https://reactjs.org/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3.3-purple?style=flat-square&logo=bootstrap)](https://getbootstrap.com/)
[![React Router](https://img.shields.io/badge/React_Router-6.26.2-red?style=flat-square&logo=react-router)](https://reactrouter.com/)
[![JSON Server](https://img.shields.io/badge/JSON_Server-1.0.0-green?style=flat-square)](https://github.com/typicode/json-server)
[![License](https://img.shields.io/badge/License-ITI_Project-orange?style=flat-square)](LICENSE)

## 🌟 Overview

Tech Heaven is a comprehensive e-commerce web application built with React that provides a complete online shopping experience for smartphones. The platform features user authentication, product management with full CRUD operations, shopping cart functionality, and an intuitive admin dashboard. Built as an ITI Final Project, it demonstrates modern web development practices with a focus on user experience and responsive design.

### ✨ Key Features

- **🛍️ Complete Shopping Experience**: Browse, search, filter, and purchase smartphones
- **🔐 Secure Authentication**: User registration, login with Google OAuth integration
- **📦 Product Management**: Full CRUD operations for product catalog
- **🛒 Shopping Cart**: Add to cart, manage quantities, and checkout
- **👨‍💼 Admin Dashboard**: Product and user management interface
- **📱 Responsive Design**: Seamless experience across all devices
- **🎨 Modern UI**: Beautiful interface with Bootstrap and Material-UI components
- **🔔 Real-time Notifications**: Toast notifications for user actions
- **⭐ Product Ratings**: Display customer reviews and ratings
- **💰 Discount System**: Dynamic pricing with discount calculations

## 🚀 Getting Started

### Prerequisites

- **Node.js** 14.x or higher
- **npm** 6.x or higher
- **Git** for version control

### Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd PhoneStore_ITI_Final_Project-main
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start the JSON Server (Backend)**

   Open a terminal and run:

   ```bash
   npx json-server --watch data.json --port 3004
   ```

   This starts the mock backend API server on [http://localhost:3004](http://localhost:3004)

4. **Start the React Application (Frontend)**

   Open a **new terminal** (keep JSON Server running) and run:

   ```bash
   npm start
   ```

   This starts the development server on [http://localhost:3000](http://localhost:3000)

5. **Access the application**

   Open your browser and navigate to [http://localhost:3000](http://localhost:3000)

## 🏗️ Architecture

### Tech Stack

**Frontend:**

- [React 18.2.0](https://reactjs.org/) - JavaScript library for building user interfaces
- [React Router DOM 6.26.2](https://reactrouter.com/) - Declarative routing for React
- [Bootstrap 5.3.3](https://getbootstrap.com/) - CSS framework for responsive design
- [React-Bootstrap 2.10.4](https://react-bootstrap.github.io/) - Bootstrap components built with React
- [Material-UI 5.16.7](https://mui.com/) - React component library
- [Swiper 11.1.14](https://swiperjs.com/) - Modern mobile touch slider
- [FontAwesome 6.6.0](https://fontawesome.com/) - Icon library

**Authentication & Social:**

- [Google OAuth](https://www.npmjs.com/package/@react-oauth/google) - Google authentication integration
- [EmailJS](https://www.emailjs.com/) - Email service integration

**State Management & HTTP:**

- React Context API - Global state management
- [Axios 1.7.7](https://axios-http.com/) - Promise-based HTTP client

**UI Enhancements:**

- [React Hot Toast](https://react-hot-toast.com/) - Toast notifications
- [React Toastify](https://fkhadra.github.io/react-toastify/) - Notification system
- [React Scroll](https://www.npmjs.com/package/react-scroll) - Smooth scrolling
- [Google Map React](https://www.npmjs.com/package/google-map-react) - Google Maps integration

**Backend (Mock):**

- [JSON Server 1.0.0](https://github.com/typicode/json-server) - Full fake REST API

### Project Structure

```
PhoneStore_ITI_Final_Project-main/
├── public/                       # Static files
│   ├── index.html
│   ├── logo.png
│   ├── logo.svg
│   ├── manifest.json
│   └── robots.txt
├── src/
│   ├── Components/               # React components
│   │   ├── CRUD/                # Product CRUD operations
│   │   │   ├── Shop.jsx         # Product listing with search & filter
│   │   │   ├── Details.jsx      # Product detail view
│   │   │   ├── EditProduct.jsx  # Edit product form
│   │   │   ├── addProduct.jsx   # Add new product form
│   │   │   ├── ProductCard.jsx  # Product card component
│   │   │   ├── ProductTable.jsx # Product table view
│   │   │   └── UserManagement.jsx # Admin user management
│   │   ├── Shared/              # Shared components
│   │   │   ├── Navbar.jsx       # Navigation bar
│   │   │   ├── Footer.jsx       # Footer component
│   │   │   └── CartCount.js     # Shopping cart counter
│   │   ├── Users/               # Authentication
│   │   │   ├── Login.jsx        # Login page with OAuth
│   │   │   └── Register.jsx     # User registration
│   │   ├── Home.jsx             # Landing page
│   │   ├── Cart.jsx             # Shopping cart
│   │   ├── Aboutus.jsx          # About us page
│   │   ├── Contactus.jsx        # Contact form with EmailJS
│   │   ├── BrandSwiper.jsx      # Brand carousel slider
│   │   ├── NotFound.jsx         # 404 error page
│   │   ├── ScrollToTop.jsx      # Scroll utility
│   │   └── localBrands.js       # Brand data
│   ├── ContextAPIs/             # Context providers
│   │   └── ProductsContext.jsx  # Products & cart state
│   ├── Images/                  # Image assets
│   │   ├── brand logos
│   │   ├── team photos
│   │   └── icons
│   ├── Styles/                  # CSS modules
│   │   ├── home.module.css
│   │   ├── shop.module.css
│   │   ├── Navbar.module.css
│   │   ├── Footer.module.css
│   │   └── [other styles]
│   ├── App.js                   # Main application component
│   ├── App.css                  # Global app styles
│   ├── index.js                 # Application entry point
│   └── index.css                # Global CSS
├── data.json                     # Mock database
├── package.json                  # Dependencies and scripts
├── package-lock.json
└── README.md                     # Documentation
```

## 🛍️ Features in Detail

### For Customers

#### Home Page

- Welcoming hero section with call-to-action
- Featured products showcase (top 3 products)
- "Why Choose Us" section highlighting:
  - 24/7 Customer Service
  - Customer Testimonials
  - Quality Commitment
  - Warranty Included
- Brand carousel with Swiper
- Integrated contact form

#### Product Browsing

- **Shop Page**: View all available smartphones
- **Search Functionality**: Find products by name
- **Brand Filtering**: Filter by manufacturer (Apple, Samsung, Google, OnePlus, etc.)
- **Product Cards**: Display with image, name, price, discount, rating, and stock
- **Product Details**: Comprehensive information including:
  - High-quality product images
  - Price with discount calculations
  - Stock availability
  - Customer ratings
  - Detailed description
  - Add to cart button

#### Shopping Cart

- Add/remove products
- View cart items
- Quantity management
- Total price calculation
- Discount application
- Checkout process

#### User Account

- **Registration**: Create new account with validation
- **Login**: Email/password or Google OAuth
- **Profile Management**: Update personal information
- **Order History**: View past purchases

#### Contact & Support

- Contact form with EmailJS integration
- Google Maps location integration
- Customer service information
- Social media links

### For Administrators

#### Product Management

- **Add Products**:
  - Upload product images
  - Set pricing and discounts
  - Manage stock levels
  - Define categories and brands
  - Add descriptions and ratings
- **Edit Products**: Update any product information
- **Delete Products**: Remove products from catalog
- **View Products**: Table and card views

#### User Management

- View all registered users
- User account information
- Role management (admin/user)
- User activity monitoring

## 🔐 Authentication

### Default Login Credentials

**Admin Account:**

- Username: `admin`
- Password: `admin`
- Email: `Admin@admin.com`
- Role: Administrator

**Test User Account:**

- Username: `mohamed`
- Password: `123`
- Email: `mohamed@gmail.com`
- Role: Regular User

### Authentication Features

- JWT-based session management
- Google OAuth integration
- Form validation
- Password security
- Role-based access control
- Persistent login with localStorage

## 🌐 API Endpoints

The JSON Server provides a REST API for data management:

### Products

- `GET /products` - Get all products
- `GET /products/:id` - Get product by ID
- `POST /products` - Add new product
- `PUT /products/:id` - Update product
- `PATCH /products/:id` - Partial update
- `DELETE /products/:id` - Delete product

### Users

- `GET /User` - Get all users
- `GET /User/:id` - Get user by ID
- `POST /User` - Register new user
- `PUT /User/:id` - Update user
- `DELETE /User/:id` - Delete user

### Cart/Orders

- `GET /orderItem` - Get cart items
- `POST /orderItem` - Add item to cart
- `DELETE /orderItem/:id` - Remove from cart

## 🎨 UI/UX Features

### Design Elements

- **Responsive Layout**: Mobile-first design approach
- **Modern Card Design**: Clean product cards with hover effects
- **Glass Morphism**: Modern UI effects on key components
- **Smooth Animations**: Page transitions and component animations
- **Color Scheme**: Professional color palette with brand consistency
- **Typography**: Readable fonts with proper hierarchy

### User Experience

- **Toast Notifications**: Immediate feedback for all actions
- **Loading States**: Visual feedback during data fetching
- **Error Handling**: Graceful error messages
- **Form Validation**: Real-time input validation
- **Smooth Scrolling**: Enhanced navigation experience
- **Scroll to Top**: Quick navigation button
- **404 Page**: Custom not-found page

### Accessibility

- Semantic HTML structure
- Keyboard navigation support
- ARIA labels where applicable
- Color contrast compliance
- Responsive font sizing

## 📱 Responsive Design

The application is fully responsive and optimized for:

- **Desktop** (1200px+): Full-featured experience with multi-column layouts
- **Laptop** (992px-1199px): Optimized layout for medium screens
- **Tablet** (768px-991px): Touch-friendly interface with adjusted layouts
- **Mobile** (< 768px): Single-column layout with mobile-optimized navigation

## 🧪 Available Scripts

### Development

```bash
npm start          # Start development server (port 3000)
npm test           # Run test suite
npm run build      # Build for production
npm run eject      # Eject from Create React App (irreversible)
```

### Backend

```bash
npx json-server --watch data.json --port 3004  # Start mock API server
```

### Deployment

```bash
npm run predeploy  # Build before deployment
npm run deploy     # Deploy to GitHub Pages
```
