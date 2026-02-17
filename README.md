# 🛍️ DigiShop - E-Commerce Store with Next.js

A complete e-commerce store similar to Digikala, built with **Next.js 16**, **TypeScript**, and **Tailwind CSS**. This project includes authentication system, product management, shopping cart, and a modern responsive user interface.

![Next.js](https://img.shields.io/badge/Next.js-16.1.6-black?style=for-the-badge&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.0-38bdf8?style=for-the-badge&logo=tailwind-css)
![Prisma](https://img.shields.io/badge/Prisma-7.4.0-2D3748?style=for-the-badge&logo=prisma)

## ✨ Features

- 🎨 **Modern & Professional Design** - Beautiful and user-friendly UI with Tailwind CSS
- 📱 **Fully Responsive** - Compatible with all devices (mobile, tablet, desktop)
- 🔐 **Authentication System** - User login and registration with bcrypt
- 🛒 **Shopping Cart** - Manage cart and add/remove products
- 📦 **Product Management** - Admin panel for adding, editing, and deleting products
- 🏷️ **Product Categories** - Filter and search by category
- 🖼️ **Image Loading from API** - Using Unsplash for product images
- 🎯 **Mega Menu** - Professional menu with various categories
- ⚡ **Fast & Optimized** - Using Next.js App Router and Server Components
- 🗄️ **Database** - Prisma support with SQLite (can be changed to PostgreSQL/MySQL)

## 🚀 Quick Start

### Prerequisites

- Node.js 18+
- npm or yarn

### Installation & Setup

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/digishop.git
cd digishop

# Install dependencies
npm install

# Run development server
npm run dev
```

The project will be available at [http://localhost:3000](http://localhost:3000).

### Database Setup (Optional)

```bash
# Create database and run migrations
npx prisma migrate dev

# Seed database with sample data
npm run db:seed
```

## 📁 Project Structure

```
shop/
├── src/
│   ├── app/              # Pages and API routes
│   │   ├── api/         # API endpoints
│   │   ├── admin/       # Admin panel
│   │   ├── login/       # Login/Register page
│   │   ├── products/    # Product pages
│   │   └── cart/        # Shopping cart
│   ├── components/      # React components
│   ├── data/           # Demo data
│   └── lib/            # Helper libraries
├── prisma/             # Schema and migrations
└── public/            # Static files
```

## 🎯 Main Pages

- **Home Page** (`/`) - Display featured and recommended products
- **Products** (`/products`) - Complete product list with category filter
- **Product Details** (`/products/[id]`) - Complete information for each product
- **Shopping Cart** (`/cart`) - Manage shopping cart
- **Login/Register** (`/login`) - User authentication
- **Admin Panel** (`/admin`) - Product management (requires admin access)

## 🔑 Access Credentials

### Default Admin User
- **Email:** `admin@digishop.com`
- **Password:** `admin123`

> ⚠️ Note: Make sure to change the password in production environment!

## 🛠️ Technologies Used

- **Framework:** Next.js 16 (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS 4
- **Database:** Prisma + SQLite (changeable)
- **Authentication:** bcryptjs
- **UI Components:** Custom Components with Tailwind

## 📡 API Endpoints

### Products
- `GET /api/products` - Get list of products
- `GET /api/products?category=...` - Filter by category
- `GET /api/products/[id]` - Get product details
- `POST /api/products` - Add product (requires auth)
- `PUT /api/products/[id]` - Update product
- `DELETE /api/products/[id]` - Delete product

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login

### Categories
- `GET /api/categories` - Get list of categories

### Shopping Cart
- `GET /api/cart` - Get shopping cart
- `POST /api/cart` - Add to cart
- `DELETE /api/cart` - Clear cart

## 🎨 UI/UX Features

- ✨ Smooth and fluid animations
- 🎯 Mega menu for quick access
- 📱 Mobile-first design
- 🌙 Ready for dark mode
- ⚡ Fast loading with Next.js SSR/SSG

## 📝 Notes

This project is a **demo** and is built for learning and development purposes. For production use:

- ✅ Use a real database (PostgreSQL/MySQL)
- ✅ Implement JWT for authentication
- ✅ Add rate limiting
- ✅ Complete input validation
- ✅ Write unit and E2E tests
- ✅ Set up CI/CD pipeline

## 🤝 Contributing

Contributions, suggestions, and bug reports are welcome! Please:

1. Fork the project
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

## 👨‍💻 Developer

Built with ❤️ by **Alireza Zolfaghari**

---

⭐ If this project was helpful to you, give it a star!
