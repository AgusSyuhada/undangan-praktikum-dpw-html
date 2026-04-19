# Undangan Pernikahan Digital & Admin Dashboard

Proyek ini adalah aplikasi web statis untuk Undangan Pernikahan Digital yang dilengkapi dengan Panel Admin (Dashboard) terintegrasi. Proyek ini dibuat untuk memudahkan pengelolaan tamu, RSVP, dan konten undangan secara dinamis melalui antarmuka admin yang responsif.

## 🚀 Teknologi yang Digunakan

* **HTML5** - Struktur dasar halaman.
* **Tailwind CSS (via CDN)** - Framework CSS untuk styling yang cepat dan responsif.
* **Vanilla JavaScript** - Untuk interaktivitas DOM (Modal, navigasi sidebar, show/hide password, countdown, dll).
* **FontAwesome (v6.4.0)** - Ikon vektor untuk antarmuka pengguna.
* **Google Fonts** - Menggunakan font *Poppins* untuk UI/Dashboard dan *Great Vibes* untuk tipografi undangan.

## ✨ Fitur Utama

### 1. Halaman Undangan (Client-Side)
* **Cover Interaktif:** Halaman sampul dengan nama tamu yang dipersonalisasi melalui parameter URL (`?to=Nama Tamu`).
* **Background Music:** Pemutar musik latar otomatis (autoplay) saat undangan dibuka, dilengkapi tombol putar/jeda (Floating Action Button).
* **Countdown Timer:** Penghitung waktu mundur yang presisi menuju hari-H acara.
* **Integrasi Google Maps:** Menampilkan peta lokasi acara secara langsung menggunakan iframe.
* **Buku Tamu & RSVP:** Form bagi tamu untuk mengonfirmasi kehadiran dan memberikan ucapan, beserta daftar ucapan yang dapat digulir (custom scrollbar).
* **Wedding Gift:** Fitur salin nomor rekening (Copy to Clipboard) untuk hadiah digital.

### 2. Panel Admin (Dashboard)
* **Sistem Login:** Mendukung login menggunakan *Username* ataupun *Email*, dilengkapi dengan fitur "Show/Hide Password".
* **Layout Responsif:** * Di mode Desktop: Sidebar navigasi tetap (fixed).
    * Di mode Mobile: Sidebar bersembunyi secara otomatis (off-canvas) dan dapat dipanggil menggunakan *Hamburger Menu* dengan efek *overlay* gelap.
* **Manajemen RSVP:** Tabel untuk melihat konfirmasi kehadiran dan ucapan dari tamu.
* **Manajemen Tamu:** Fitur tambah, edit, dan hapus tamu. Dilengkapi tombol *Copy Link* untuk menyalin URL undangan unik masing-masing tamu secara otomatis.
* **Manajemen Admin:** Fitur untuk mengelola pengguna (admin) yang memiliki akses ke dashboard. Form edit/tambah mendukung fitur "Show/Hide Password".
* **Manajemen Konten:** Memungkinkan admin mengubah teks, tautan gambar, dan iframe secara dinamis. Menggunakan antarmuka navigasi *Tabs* yang responsif.
* **Tabel Responsif:** Seluruh tabel data dibungkus agar dapat digulir secara horizontal (scrollable) pada layar perangkat seluler (HP) sehingga tata letak tidak rusak.
* **Keamanan Aksi:** Menggunakan *Modal Konfirmasi* interaktif untuk setiap tindakan krusial seperti Menghapus Data dan Logout.

## 📁 Struktur Direktori

```text
📂 undangan-praktikum-dpw
├── 📄 index.html             # Halaman utama undangan digital
├── 📄 login.html             # Halaman login untuk Admin
├── 📄 README.md              # Dokumentasi proyek
└── 📂 dashboard              # Kumpulan halaman Panel Admin
    ├── 📄 content-form.html  # Form edit konten spesifik
    ├── 📄 content.html       # Tabel manajemen isi halaman undangan
    ├── 📄 guest-form.html    # Form tambah/edit nama tamu
    ├── 📄 guests.html        # Tabel daftar tamu & salin link undangan
    ├── 📄 rsvp.html          # Tabel data kehadiran dan ucapan (Landing dashboard)
    ├── 📄 user-form.html     # Form tambah/edit data admin
    └── 📄 users.html         # Tabel daftar pengguna/admin
```

## 🛠️ Cara Penggunaan

1.  **Clone / Unduh Repository:** Unduh seluruh file proyek ini ke dalam komputer Anda.
2.  **Buka Halaman Undangan:** Buka file `index.html` di browser Anda untuk melihat tampilan undangan. Anda bisa menambahkan `?to=Nama+Tamu` di akhir URL untuk melihat fitur nama tamu dinamis.
3.  **Akses Dashboard Admin:** * Buka file `login.html` di browser.
    * Login menggunakan data *dummy* berikut:
        * **Username / Email:** `admin` atau `admin@undangan.com`
        * **Password:** `1234`
4.  **Eksplorasi Dashboard:** Anda bisa menguji fungsionalitas form, tombol salin link, modal hapus, hingga tampilan responsif dengan mengecilkan jendela browser atau menggunakan *developer tools* (mode mobile).

---