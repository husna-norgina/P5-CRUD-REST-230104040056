# 🌐 Praktikum #5 — Web Service Engineering

Membangun RESTful CRUD API berbasis Express.js dengan struktur modular.
Project ini mengimplementasikan operasi CRUD untuk resource `products`.

**Topik:** Membangun RESTful CRUD API dengan Express.js

---

## 🧑‍🎓 Informasi Mahasiswa

| Informasi        | Data                                           |
|------------------|------------------------------------------------|
| Mata Kuliah      | Web Service Engineering                        |
| Dosen Pengampu   | Muhayat, M.IT                                  |
| Praktikum        | P5 - Membangun RESTful CRUD API dengan Express |
| Nama Mahasiswa   | Husna Norgina                                  |
| NIM              | 230104040056                                   |
| Kelas            | TI23B                                          |
| Tanggal Praktikum| 03-11-2025                                     |

---

## 🎯 Tujuan Praktikum

1. Membangun RESTful API sederhana menggunakan Express.js.
2. Menerapkan operasi dasar CRUD (Create, Read, Update, Delete).
3. Menggunakan HTTP method & status code secara tepat.
4. Mengetahui struktur dasar modular server API pada Node.js.
5. Menghasilkan response JSON konsisten dan valid.

---

## 🛠 Tools & Environment

* Node.js 18+
* npm
* Express.js
* VSCode
* Nodemon (Dev Dependency)
* Postman / Thunder Client
* Git (opsional)

---

## 🧩 Skenario Sistem

Membangun RESTful API untuk resource: **products**

Endpoint Base:

```
/api/products
```

CRUD implemented:

| Method | Path              | Deskripsi          |
| ------ | ----------------- | ------------------ |
| GET    | /api/products     | Ambil semua produk |
| GET    | /api/products/:id | Ambil produk by ID |
| POST   | /api/products     | Tambah produk      |
| PUT    | /api/products/:id | Update produk      |
| DELETE | /api/products/:id | Hapus produk       |

---

## ⚙️ Langkah Implementasi Singkat

1. Membuat folder project `P5-CRUD-REST-230104040056`
2. `npm init -y`
3. Install dependency:

```
npm install express
npm install nodemon --save-dev
```

4. Struktur folder:

```
src/
 ├─ routes/
 ├─ data/
 └─ app.js
```

5. Tulis CRUD logic pada `products.routes.js`
6. Register route di `app.js`:

```
app.use('/api/products', productRoutes)
```

7. Run server:

```
npm run dev
```

---

## 🧾 Evidence Pengujian Endpoint (Postman)

| Endpoint                 | Status                   |
| ------------------------ | ------------------------ |
| GET /api/products        | ✅ 200 OK                 |
| GET /api/products/:id    | ✅ 200 OK / 404 Not Found |
| POST /api/products       | ✅ 201 Created            |
| PUT /api/products/:id    | ✅ 200 OK / 404 Not Found |
| DELETE /api/products/:id | ✅ 200 OK / 404 Not Found |

> Evidence screenshot disimpan di folder: `./evidence/`

---

## 📊 Analisis

API CRUD berjalan dengan benar, status response sesuai standar HTTP. Struktur project modular membuat maintain & scale lebih mudah. Validasi & error handling masih basic, improvement akan dilakukan pada praktikum selanjutnya.

---

## ✅ Kesimpulan

RESTful CRUD API berhasil dibuat menggunakan Express.js dan seluruh endpoint teruji berhasil.

---

## 📌 Checklist Praktikum

* ✅ Struktur project sesuai
* ✅ Endpoint CRUD lengkap dan berfungsi
* ✅ Response JSON valid
* ✅ Status code sesuai standar REST
* ✅ Evidence pengujian tersedia

---
