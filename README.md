# 🍕 RestaurantOS - Food Delivery App

A full-stack **Food Delivery Application** built with React, Node.js, and MongoDB. Features multi-role access: Customer ordering, Restaurant Manager dashboard, and Admin controls.

---

## 🎯 Project Overview

RestaurantOS is a complete food delivery platform where:
- **Customers** browse restaurants, order food, track deliveries
- **Managers** add/edit menu items, manage orders, update status
- **Admins** control users, restaurants, and system-wide analytics

---

## ✨ Key Features

### 👤 Customer Portal
- Browse restaurant listings with search & filters
- View detailed menus with images and pricing
- Add items to cart with quantity controls
- Checkout with delivery address & payment info
- Track order status in real-time
- View order history

### 👨‍💼 Manager Dashboard
- **Orders Tab**: View incoming orders with status management (preparing → ready → delivered)
- **Menu Management Tab**: Add/edit/delete categories and items with images
- Real-time order notifications
- Mark items as sold out
- Filter and sort orders

### 🛡️ Admin Dashboard
- **Users Tab**: Manage all users and assign roles
- **Restaurants Tab**: Monitor all restaurants, performance stats
- **Orders Tab**: System-wide order analytics and management

---

## 🛠️ Tech Stack

**Frontend:**
- React.js + Vite
- Context API for state management
- Tailwind CSS for styling

**Backend:**
- Node.js + Express
- MongoDB for database
- JWT for authentication
- Multer for file uploads

**Deployment:**
- Frontend: Vercel
- Backend: Heroku/Railway

---

## 📦 Installation & Setup

### Prerequisites
- Node.js 16+
- MongoDB (local or Atlas)
- Git

### Backend Setup
```bash
cd backend
npm install
cp .env.example .env
# Add your MongoDB URI and JWT secret to .env
npm run dev
```

### Frontend Setup
```bash
cd frontend
npm install
cp .env.example .env
# Add your backend API URL to .env
npm run dev
```

### Access Points
- **Customer**: `http://localhost:5173`
- **Manager**: `http://localhost:5173/manager/orders`
- **Admin**: `http://localhost:5173/admin/dashboard`

---

## 📸 Screenshots

### Home Page
![Home Page](screenshots/home-page.png)
Customer dashboard with hero section and popular restaurants

### Restaurant Menu
![Restaurant Menu](screenshots/restaurant-menu.png)
Browse menu items with descriptions, prices, and "Add to Cart" buttons

### Manager Menu Management
![Manager Menu](screenshots/manager-menu.png)
Add/edit menu items and categories with real images

### Manager Orders
![Manager Orders](screenshots/manager-orders.png)
Real-time order management with status tracking and action buttons

### Admin Dashboard
![Admin Users](screenshots/admin-users.png)
Manage all users, assign roles, and control platform access

---

## 🚀 Usage Guide

### For Customers
1. Browse restaurants on homepage
2. Click restaurant to view menu
3. Add items to cart
4. Proceed to checkout
5. Enter delivery address and payment info
6. Track order status

### For Restaurant Managers
1. Login with manager credentials
2. Go to **Orders** tab to manage incoming orders
3. Go to **Menu** tab to:
   - Add new categories (e.g., Appetizers, Mains)
   - Add menu items with image URLs and pricing
   - Edit or delete existing items
   - Mark items as sold out

### For Admins
1. Access admin dashboard
2. **Users Tab**: View/edit user roles
3. **Restaurants Tab**: Monitor restaurant performance
4. **Orders Tab**: View system-wide analytics

---

## 🔐 Default Test Accounts

| Role | Email | Password |
|------|-------|----------|
| Customer | customer@example.com | password123 |
| Manager | manager@example.com | password123 |
| Admin | admin@example.com | password123 |

---

## 📝 Environment Variables

### Backend (.env)
```
PORT=5000
MONGODB_URI=mongodb+srv://user:pass@cluster.mongodb.net/dbname
JWT_SECRET=your_secret_key
NODE_ENV=development
```

### Frontend (.env)
```
VITE_API_URL=http://localhost:5000/api
```

---

## 🐛 Troubleshooting

**Issue: "Cannot connect to backend"**
- Ensure backend is running on port 5000
- Check VITE_API_URL in frontend .env
- Verify MongoDB connection

**Issue: "Menu items not showing"**
- Check if manager has added items via Menu Management tab
- Verify image URLs are accessible
- Check browser console for errors

**Issue: "Orders not updating"**
- Refresh page to sync latest orders
- Check manager login status
- Verify MongoDB is running

---

## 🤝 Contributing

1. Create feature branch: `git checkout -b feature/your-feature`
2. Commit changes: `git commit -m "Add your feature"`
3. Push: `git push origin feature/your-feature`
4. Create Pull Request

---

## 📞 Support

For issues or questions, contact: support@restaurantos.com

---

## 📄 License

MIT License - see LICENSE file for details

---

**Built with ❤️ for food lovers**
