# LaraPress---Aplikasi-Blog-Sederhana
<p align="center">
  <a href="https://laravel.com" target="_blank">
    <img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo">
  </a>
</p>

<p align="center">
  <a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
  <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
  <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
  <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# 📰 LaraPress - Aplikasi Blog Sederhana

**LaraPress** adalah aplikasi blog sederhana yang dikembangkan menggunakan **Laravel 12** sebagai sarana **pembelajaran** dan **pengembangan keterampilan web development**.

<img width="1919" height="1079" alt="Image" src="https://github.com/user-attachments/assets/4335f29c-374c-4d1c-bc41-1dd364c3534f" />
*Tampilan halaman utama LaraPress*

---

## 📋 Tentang Proyek

Proyek ini dibuat untuk mempelajari dasar-dasar framework **Laravel**, mencakup konsep seperti **routing**, **views**, dan **struktur MVC**.

---

## 🚀 Fitur yang Tersedia

### 1. Halaman Utama (Welcome Page)
- Mengubah tampilan default Laravel menjadi halaman sederhana.
- Menampilkan judul *"Selamat Datang di LaraPress"*.
- Menggunakan struktur HTML yang bersih dan minimalis.

### 2. Halaman Tentang Kami
- **Route:** `/about`
- Berisi informasi tentang LaraPress dan tujuan proyek.

### 3. Halaman Kontak
- **Route:** `/contact`
- Berisi informasi kontak pengembang.

---

## 📁 Struktur File yang Dimodifikasi

| File | Deskripsi |
|------|-----------|
| `resources/views/welcome.blade.php` | Mengubah tampilan default Laravel menjadi halaman utama sederhana. |
| `resources/views/about.blade.php` *(baru)* | View untuk halaman "Tentang Kami". |
| `resources/views/contact.blade.php` *(baru)* | View untuk halaman "Kontak". |
| `routes/web.php` | Menambahkan route baru `/about` dan `/contact`. |

---

## 🛠️ Langkah Implementasi

### 1. Modifikasi Halaman Welcome

```html
<!DOCTYPE html>
<html>
<head>
  <title>Selamat Datang di LaraPress</title>
</head>
<body>
  <h1>Selamat Datang di Blog LaraPress</h1>
  <p>Ini adalah halaman utama dari aplikasi blog kami.</p>
  <a href="/about">Lihat Halaman Tentang Kami</a>
  <br>
  <a href="/">Kembali ke Halaman Utama</a>
</body>
</html>

### 2. Tambahkan Route Baru

Route::get('/about', function () {
    return view('about');
});
Route::get('/contact', function () {
    return view('contact');
});

### 3. Buat View About

<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tentang Kami - LaraPress</title>
</head>
<body>
  <h1>Tentang LaraPress</h1>
  <p>LaraPress adalah aplikasi blog sederhana yang dikembangkan menggunakan Laravel 12.</p>
  <p>Proyek ini dibuat untuk tujuan pembelajaran dan peningkatan keterampilan web development.</p>
</body>
</html>

### 4. Buat View Contact

<!DOCTYPE html>
<html>
<head>
  <title>Kontak Kami - LaraPress</title>
</head>
<body>
  <h1>Kontak LaraPress</h1>
  <p>Nama : Muhammad Naufal Isyrafi</p>
  <p>NPM : 4523210120</p>
  <p>Email : isyrafii4523117@univpancasila.ac.id</p>
  <p>No. HP : 081277306920</p>
  <a href="/about">Lihat Halaman Tentang Kami</a>
  <br>
  <a href="/">Kembali ke Halaman Utama</a>
</body>
</html>
