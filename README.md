# FinCerdas

FinCerdas adalah aplikasi berbasis web yang membantu pengguna menganalisis risiko gagal bayar kartu kredit menggunakan teknologi Machine Learning. Aplikasi ini memungkinkan pengguna melakukan registrasi, memasukkan data keuangan, memperoleh hasil analisis risiko, serta menerima rekomendasi keuangan yang dipersonalisasi.

Proyek ini dikembangkan sebagai bagian dari **Capstone Project Coding Camp 2026** dengan mengintegrasikan Frontend, Backend REST API, dan Model Machine Learning.

🔗 **Frontend Demo:** https://anabilaa-xyz.github.io/fincerdas-frontend

🔗 **Backend API:** https://gregarious-art-production-cac2.up.railway.app

---

# 📌 Fitur Utama

### 🔐 Autentikasi Pengguna

- Registrasi akun baru
- Login menggunakan email dan password
- Proteksi endpoint menggunakan JWT

### 📊 Analisis Risiko Kredit

- Input data keuangan kartu kredit
- Integrasi dengan model Machine Learning
- Prediksi risiko gagal bayar kartu kredit

### 📈 Hasil Analisis

- Skor risiko
- Kategori risiko
- Visualisasi hasil analisis

### 💡 Rekomendasi Keuangan

- Prioritas utama
- Langkah perbaikan jangka pendek
- Strategi keuangan jangka panjang

---

# 🏗️ Arsitektur Sistem

```text
┌─────────────────┐
│    Frontend     │
│ React + Vite    │
└────────┬────────┘
         │ HTTP Request
         ▼
┌─────────────────┐
│   Backend API   │
│ Node + Express  │
└────────┬────────┘
         │
         ├─────────────► PostgreSQL (Supabase)
         │
         ▼
┌─────────────────┐
│ Machine Learning│
│ Prediction API  │
└─────────────────┘
```

---

# 🚀 Tech Stack

## Frontend

- React 19
- Vite 8
- React Router DOM 7
- Axios
- Tailwind CSS 4
- Lucide React
- GitHub Pages

## Backend

- Node.js
- Express.js
- PostgreSQL (Supabase)
- JSON Web Token (JWT)
- Bcryptjs
- Axios
- CORS
- dotenv

## Machine Learning

- Python
- FastAPI / Flask (sesuaikan dengan model ML kalian)
- Railway Deployment

---

# 📂 Struktur Repository

```text
ProjectFintech/
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
├── Backend/
│   ├── src/
│   ├── package.json
│   └── .env
│
└── README.md
```

---

# 🌐 Deployment

| Komponen | Platform | URL |
|-----------|-----------|-----------|
| Frontend | GitHub Pages | https://anabilaa-xyz.github.io/fincerdas-frontend |
| Backend API | Railway | https://gregarious-art-production-cac2.up.railway.app |
| Database | Supabase | PostgreSQL |
| Machine Learning API | Railway | https://web-production-92448.up.railway.app |

---

# ⚙️ Instalasi Lokal

## 1. Clone Repository

```bash
git clone https://github.com/deviiaulya/ProjectFintech.git
```

```bash
cd ProjectFintech
```

---

# 💻 Menjalankan Frontend

Masuk ke folder frontend:

```bash
cd frontend
```

Install dependency:

```bash
npm install
```

Buat file `.env`

```env
VITE_API_URL=https://gregarious-art-production-cac2.up.railway.app/api
```

Jalankan aplikasi:

```bash
npm run dev
```

Frontend akan berjalan pada:

```text
http://localhost:5173
```

---

# ⚙️ Menjalankan Backend

Masuk ke folder backend:

```bash
cd Backend
```

Install dependency:

```bash
npm install
```

Buat file `.env`

```env
PORT=5000

ML_API_URL=https://web-production-92448.up.railway.app

DATABASE_URL=postgresql://postgres.[project]:[password]@[host]:5432/postgres

JWT_SECRET=your_jwt_secret_key
```

Jalankan server:

```bash
npm run start
```

Backend akan berjalan pada:

```text
http://localhost:5000
```

---

# 📌 API Endpoint

Base URL:

```text
https://gregarious-art-production-cac2.up.railway.app/api
```

| Method | Endpoint | Deskripsi |
|----------|----------|----------|
| POST | `/auth/register` | Registrasi pengguna |
| POST | `/auth/login` | Login pengguna |
| GET | `/user/profile` | Profil pengguna |
| POST | `/predict` | Prediksi risiko gagal bayar |
| GET | `/analyses/history` | Riwayat analisis |
| GET | `/analyses/:id` | Detail analisis |

---

# 🔒 Authentication

Endpoint tertentu memerlukan JWT Token.

Tambahkan token pada header:

```http
Authorization: Bearer <JWT_TOKEN>
```

Token diperoleh setelah pengguna berhasil login.

---

# 🔄 Alur Penggunaan Aplikasi

```text
Landing Page
      │
      ▼
Register
      │
      ▼
Login
      │
      ▼
Dashboard
      │
      ▼
Input Data Keuangan
      │
      ▼
Machine Learning Prediction
      │
      ▼
Hasil Analisis Risiko
      │
      ▼
Rekomendasi Keuangan

```


# 👨‍💻 Tim Pengembang

| Peran | Nama |
|---------|---------|
| Frontend Developer | Anabila |
| Backend Developer | Devi Aulya Hapsari |
| Machine Learning Engineer | Samuel dan Joshua |
| Data science | Sultan dan Rachel |

---

# 🎯 Tujuan Proyek

FinCerdas dikembangkan untuk membantu masyarakat memahami tingkat risiko gagal bayar kartu kredit melalui analisis data keuangan berbasis Machine Learning serta memberikan rekomendasi keuangan yang dapat membantu pengambilan keputusan finansial yang lebih baik.

---

# 📄 Lisensi

Project ini dibuat untuk keperluan akademik dan pembelajaran dalam program Capstone Coding Camp 2026.
