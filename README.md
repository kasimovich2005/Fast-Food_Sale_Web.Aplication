<div align="center">

# 🍔 Fast-Food Sale Web Application

**A full-stack online fast food ordering platform with real-time order tracking and Stripe payment integration.**

[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white)](https://stripe.com/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)

</div>

---

## 📌 Loyiha Haqida

**Fast-Food Sale Web Application** — bu foydalanuvchilarga onlayn tarzda fast food mahsulotlarini ko'rish, savatga qo'shish, manzil kiritish va Stripe orqali xavfsiz to'lov amalga oshirish imkonini beruvchi to'liq funksional veb-platforma. Admin panel orqali barcha buyurtmalar real vaqtda boshqariladi.

---

## ✨ Asosiy Imkoniyatlar

### 👥 Foydalanuvchi
| Funksiya | Tavsif |
|---|---|
| 🔐 Autentifikatsiya | Ro'yxatdan o'tish va login (JWT) |
| 🍕 Menyu | Mahsulotlar ro'yxati va kategoriya bo'yicha filtrlash |
| 🛒 Savat | Mahsulot qo'shish / o'chirish |
| 📍 Manzil | Yetkazilish manzilini kiritish |
| 💳 To'lov | Stripe Checkout orqali xavfsiz to'lov |
| 📦 Tarix | Buyurtmalar tarixi va profil bo'limi |

### ⚙️ Admin Panel
| Funksiya | Tavsif |
|---|---|
| 🍔 Mahsulotlar | Qo'shish / Tahrirlash / O'chirish (CRUD) |
| 📋 Buyurtmalar | Barcha buyurtmalarni ko'rish va boshqarish |
| 🔄 Status | Pending → Cooking → Delivery → Delivered |
| 👤 Foydalanuvchilar | Ro'yxat va ma'lumotlar |
| 📊 Dashboard | Statistika va analitika |

---

## 📦 Buyurtma Jarayoni

```
1️⃣  Mahsulot tanlash       →  Savatga qo'shish
2️⃣  Savat tasdiqlash       →  Jami narxni ko'rish
3️⃣  Manzil kiritish        →  Yetkazilish manzili
4️⃣  Stripe Checkout        →  Xavfsiz to'lov
5️⃣  Order yaratish         →  Backend (Pending holat)
6️⃣  Status o'zgarishi      →  Admin tomonidan boshqariladi
```

---

## 🛠️ Texnologiyalar Steki

```
📁 Fast-Food-Sale-Web-Application/
├── 🎨 frontend/          # React 19 + Vite
└── 🔧 backend/           # Node.js + Express.js
```

| Qatlam | Texnologiyalar |
|---|---|
| **Frontend** | React.js 19, Vite, React Router, Axios |
| **Backend** | Node.js, Express.js, JWT Auth, Stripe SDK |
| **Database** | MongoDB, Mongoose |
| **To'lov** | Stripe API |

---

## 💾 Ma'lumotlar Bazasi Strukturasi

```js
// Foods Collection
{
  name: String,
  description: String,
  price: Number,
  image: String,
  category: String
}

// Users Collection
{
  name: String,
  email: String,
  password: String,     // hashed
  cardData: Object
}

// Orders Collection
{
  user: ObjectId,
  items: Array,
  totalAmount: Number,
  orderStatus: String,  // Pending | Cooking | Delivery | Delivered
  stripeSessionId: String,
  deliveryAddress: Object,
  createdAt: Date
}
```

---

## 📄 Sahifalar

### 👥 Foydalanuvchi Sahifalari
- **Home Page** — Asosiy sahifa, kategoriyalar va mahsulotlar
- **Categories** — Kategoriya bo'yicha filtrlash
- **Product Detail** — Mahsulot haqida batafsil ma'lumot
- **Cart** — Savat va narxlar
- **Checkout** — Manzil va to'lov
- **Order History** — Buyurtmalar tarixi
- **Profile** — Foydalanuvchi profili

### ⚙️ Admin Panel Sahifalari
- **Dashboard** — Statistika va ko'rsatkichlar
- **Products** — CRUD operatsiyalar
- **Orders Management** — Buyurtmalarni boshqarish
- **Status Control** — Holat o'zgartirish
- **Users List** — Foydalanuvchilar ro'yxati
- **Analytics** — Analitika

---

## 🚀 Loyihani Ishga Tushirish

### Talablar
- Node.js `v18+`
- MongoDB (local yoki Atlas)
- Stripe Account (API kalitlari)

### 1. Repozitoriyani klonlash

```bash
git clone https://github.com/kasimovich2005/Fast-Food_Sale_Web.Aplication.git
cd Fast-Food_Sale_Web.Aplication
```

### 2. Backend sozlash

```bash
cd backend
npm install
```

`.env` fayl yarating:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
STRIPE_SECRET_KEY=your_stripe_secret_key
```

```bash
npm run dev
```

### 3. Frontend sozlash

```bash
cd frontend
npm install
npm run dev
```

Brauzerda oching: `http://localhost:5173`

---

## ✅ Loyiha Tayyorligi

- [x] To'liq funktsional veb-platforma
- [x] Xavfsiz JWT autentifikatsiya
- [x] Stripe to'lov tizimi integratsiyasi
- [x] Admin paneli (full CRUD)
- [x] Real vaqtda buyurtma holati
- [x] Production uchun tayyor arxitektura

---

## 👤 Muallif

**Kasimovich** — [@kasimovich2005](https://github.com/kasimovich2005)

---

<div align="center">

⭐ Loyiha yoqsa, **star** bosishni unutmang!

</div>
