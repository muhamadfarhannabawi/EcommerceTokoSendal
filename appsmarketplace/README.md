# 🛍️ Apps Marketplace

Aplikasi Marketplace berbasis **Flutter** yang terintegrasi dengan **Golang (Gin Framework)** sebagai Backend, **MySQL** sebagai Database, **Firebase Authentication** untuk autentikasi pengguna, serta mendukung metode pembayaran **Global Institute Pay** dan **Cash On Delivery (COD)**.

---

# 📌 Deskripsi

Apps Marketplace merupakan aplikasi e-commerce sederhana yang memungkinkan pengguna untuk melakukan registrasi, login, melihat daftar produk, menambahkan produk ke keranjang, melakukan checkout, dan memilih metode pembayaran.

Aplikasi ini menggunakan konsep pemisahan Frontend dan Backend sehingga komunikasi dilakukan melalui REST API.

---

# ✨ Fitur

- Login menggunakan Firebase Authentication
- Registrasi akun
- Verifikasi Token Firebase ke Backend
- Menampilkan daftar produk
- Detail produk
- Menambahkan produk ke Cart
- Mengubah jumlah produk
- Checkout
- Pembayaran menggunakan:
  - Global Institute Pay
  - Cash On Delivery (COD)
- Dark Mode
- Manajemen Session Login
- REST API Integration

---

# 🛠️ Teknologi

## Frontend

- Flutter
- Dart
- Provider State Management
- Dio HTTP Client

## Backend

- Golang
- Gin Framework
- GORM

## Database

- MySQL

## Authentication

- Firebase Authentication

## Payment

- Global Institute Pay

---

# 📂 Struktur Project

```
appsmarketplace/
│
├── android/
├── ios/
├── lib/
│   ├── core/
│   ├── features/
│   ├── services/
│   ├── providers/
│   ├── models/
│   └── main.dart
│
├── web/
├── pubspec.yaml
└── README.md
```

---

# ⚙️ Cara Menjalankan Project

## 1. Clone Repository

```bash
git clone https://github.com/username/appsmarketplace.git
```

Masuk ke folder project

```bash
cd appsmarketplace
```

---

## 2. Install Dependency

```bash
flutter pub get
```

---

## 3. Jalankan Backend

Masuk ke folder backend

```bash
go run main.go
```

Backend berjalan pada

```
http://localhost:8080
```

---

## 4. Import Database

- Buat database MySQL
- Import file SQL
- Pastikan tabel:
  - users
  - products
  - orders
  - order_items

---

## 5. Konfigurasi Firebase

Jalankan

```bash
flutterfire configure
```

Kemudian pastikan file

```
lib/firebase_options.dart
```

telah dibuat.

---

## 6. Jalankan Flutter

Android

```bash
flutter run
```

Web

```bash
flutter run -d chrome
```

---

# 🔗 REST API

## Authentication

```
POST /v1/auth/login
POST /v1/auth/register
POST /v1/auth/verify-token
```

## Product

```
GET /v1/products
GET /v1/products/:id
```

## Cart

```
POST /v1/cart
GET /v1/cart
```

## Order

```
POST /v1/orders
GET /v1/orders
```

---

# 💾 Database

Database menggunakan **MySQL**.

Contoh tabel utama:

- users
- products
- orders
- order_items

---

# 👨‍💻 Developer

Nama : **Muhamad Farhan Nabawi**

Universitas : **Global Institute**

Program Studi : **Teknik Informatika**

---

# 📄 Lisensi

Project ini dibuat untuk keperluan pembelajaran dan tugas kuliah.