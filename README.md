# Kavan_creations
# Kavan Creations E-Commerce Platform

A custom e-commerce web application built with Django (backend) and React (frontend) for showcasing and selling high-quality handmade Ghanaian products in fashion, carpentry, bead-making, and shoemaking.

---

## 🚀 Features
- 🌍 Homepage with featured products and artisan story
- 🛍️ Product catalog by category (Fashion, Carpentry, Beads, Shoes)
- 🔎 Product detail pages with images, description, price
- 🛒 Add to cart, manage cart items
- 💳 Checkout page
- 👤 User authentication (register/login)
- 🧾 Order placement and history
- 🛠️ Admin dashboard for managing products & orders

---

## 🧰 Tech Stack

### Frontend:
- React (with Vite or Create React App)
- Tailwind CSS (for styling)
- Axios (for API requests)
- React Router DOM
- Context API (for cart/user state)

### Backend:
- Django
- Django REST Framework
- PostgreSQL
- Djoser (for user auth)
- Django CORS Headers

### Deployment (Optional):
- Backend: Render / Railway / DigitalOcean
- Frontend: Vercel / Netlify
- Media: Cloudinary / S3

---

## 📦 Installation Instructions

### 1. Backend Setup
```bash
# Create virtual environment
python3 -m venv env
source env/bin/activate  # Windows: env\Scripts\activate

# Install dependencies
pip install django djangorestframework psycopg2-binary djoser django-cors-headers

# Start project & apps
django-admin startproject kavan_backend
cd kavan_backend
python manage.py startapp products
python manage.py startapp users
python manage.py startapp orders

# Configure settings, add apps and middleware
# Apply migrations & create superuser
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser

# Run the server
python manage.py runserver
```

### 2. Frontend Setup
```bash
# Create React app
npm create vite@latest kavan-frontend --template react
cd kavan-frontend
npm install

# Install dependencies
npm install axios react-router-dom tailwindcss postcss autoprefixer
npx tailwindcss init -p

# Configure Tailwind (tailwind.config.js + index.css)

# Start development server
npm run dev
```

---

## 📁 Project Structure

```
kavan-backend/
├── kavan_backend/
├── products/
├── users/
├── orders/
└── media/

kavan-frontend/
├── src/
│   ├── components/
│   ├── pages/
│   ├── services/
│   ├── context/
│   └── App.js
```

---

## ✅ APIs Overview
- `/api/products/` – All products
- `/api/categories/` – Product categories
- `/api/auth/` – Register/login/logout
- `/api/orders/` – User orders

---

## 🔐 Authentication (Djoser)
- `POST /auth/users/` – Register
- `POST /auth/token/login/` – Login
- `POST /auth/token/logout/` – Logout

---

## 🔗 To Do / Next Steps
- [ ] Implement Order API
- [ ] Add Image Upload Support (Cloudinary or local media)
- [ ] Add Mobile Money / Stripe Payment
- [ ] Deploy backend and frontend
- [ ] Add email notifications (SendGrid)

---

## 🤝 Contributing
Feel free to fork this project and enhance it. PRs are welcome!

---

## 📬 Contact
**Founder:** Igoche, Kavan Creations  
📧 Email: [your-email@example.com]  
🌍 Location: Ghana / Germany

---

Made with ❤️ for African artisans.
