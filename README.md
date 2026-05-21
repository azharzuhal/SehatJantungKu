# ❤️ SehatJantungku

![Kotlin](https://img.shields.io/badge/Kotlin-1.9.0-purple?style=flat&logo=kotlin)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-M3-green?style=flat&logo=android)
![Firebase](https://img.shields.io/badge/Firebase-Auth%20%7C%20Firestore-orange?style=flat&logo=firebase)

**SehatJantungku** adalah aplikasi kesehatan berbasis Android yang dirancang untuk membantu pengguna memantau kesehatan jantung, menilai risiko penyakit kardiovaskular (CVD), serta menyediakan program diet dan edukasi kesehatan yang terpersonalisasi.

---

## 📺 Demo Aplikasi

Untuk melihat visualisasi antarmuka dan alur kerja aplikasi secara langsung, Anda dapat menonton video demonstrasi di bawah ini:

👉 **[Tonton Video Demo SehatJantungku di YouTube](https://youtu.be/p1N6NGliUGI)**

---

## ✨ Fitur Unggulan

### 🔐 Autentikasi & Keamanan
* **Sign Up & Sign In**: Registrasi aman menggunakan Email & Password via Firebase Auth.
* **Manajemen Akun**: Fitur ganti password dan pemulihan akun (Forgot Password).
* **Hapus Akun Permanen**: Mekanisme penghapusan data yang aman dengan verifikasi ulang (Re-authentication).

### 🩺 Kesehatan Jantung
* **Kalkulator Risiko CVD**: Algoritma pintar untuk menghitung risiko penyakit jantung berdasarkan data kesehatan pengguna.
* **Analisis Hasil**: Memberikan klasifikasi risiko (Rendah/Sedang/Tinggi) beserta saran medis.

### 🥗 Hidup Sehat
* **Program Diet Harian**: Rencana makan yang disesuaikan untuk kesehatan jantung.
* **Edukasi**: Akses ke artikel-artikel kesehatan terpercaya.
* **Smart Assistant**: Chatbot interaktif untuk konsultasi ringan seputar kesehatan.

---

## 🛠️ Tech Stack

Aplikasi ini dibangun dengan teknologi modern Android Development:

| Kategori | Teknologi |
| :--- | :--- |
| **Bahasa** | [Kotlin](https://kotlinlang.org/) |
| **UI Toolkit** | [Jetpack Compose (Material 3)](https://developer.android.com/jetpack/compose) |
| **Arsitektur** | MVVM (Model-View-ViewModel) |
| **Backend** | [Firebase Authentication](https://firebase.google.com/products/auth) & [Firestore](https://firebase.google.com/products/firestore) |
| **Navigasi** | Jetpack Navigation Compose |
| **Async** | Coroutines & Flow |

---

## 📂 Struktur Proyek

```plaintext
com.example.sehatjantungku
├── data
│   ├── model          # Data Class (User, DietPlan, dll)
│   └── repository     # Penghubung ke Firebase (AuthRepository)
├── ui
│   ├── screens        # Halaman UI (Login, Home, CVD, Profile)
│   ├── components     # Widget reusable (BottomBar, CustomButton)
│   ├── viewmodel      # Logika Bisnis (AuthViewModel, dll)
│   └── theme          # Tema & Styling Aplikasi
└── utils              # Helper & Extensions
