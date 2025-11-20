# 📄 TEMPLATE LAPORAN PROYEK: PENGEMBANGAN WEB SERVER DAN APLIKASI SEDERHANA

**Proyek:** [JUDUL PROYEK KELOMPOK KALIAN]

Proyek ini dibuat untuk memenuhi tugas mata pelajaran **[NAMA MATA PELAJARAN]** mengenai *deployment* dan konfigurasi *web server* serta implementasi keamanan SSL.

---

### 1. Informasi Kelompok dan Spesifikasi Server

| Peran | Nama Anggota | Halaman Profil di Server (Link Lokal) |
| :--- | :--- | :--- |
| **Ketua Kelompok** | [Nama Lengkap Ketua] | `https://[IP_SERVER]/[nama_ketua]` |
| Anggota 1 | [Nama Lengkap Anggota 1] | `https://[IP_SERVER]/[nama_anggota_1]` |
| Anggota 2 | [Nama Lengkap Anggota 2] | `https://[IP_SERVER]/[nama_anggota_2]` |
| **Web Server yang Dipilih** | **[Apache2 / Nginx / OpenLiteSpeed]** |
| **Versi PHP yang Dipakai** | **[mod_php / php-fpm / lsphp]** |
| **Alamat IP Server** | `[Tuliskan Alamat IP Lokal Server]` |
| **Sistem Operasi** | Debian Trixie (12.x) |

---

### 2. Dokumentasi Teknis dan Langkah-Langkah Pengerjaan

#### 2.1. Persiapan Dasar (Debian Trixie di VMware)

1.  Melakukan *update* dan *upgrade* sistem.
    ```bash
    sudo apt update && sudo apt upgrade -y
    ```
2.  Memastikan konfigurasi jaringan (NAT/Host-Only) sudah benar.

#### 2.2. Instalasi dan Konfigurasi Web Server

Kami menggunakan **[NAMA WEB SERVER]**. Berikut langkah-langkah utamanya:

* **Instalasi:**
    ```bash
    # [Tuliskan perintah instalasi Web Server Kalian, contoh: sudo apt install nginx -y]
    ```
* **Konfigurasi Virtual Host/Server Block:**
    [Jelaskan secara singkat penyesuaian konfigurasi yang Kalian lakukan pada file utama].

#### 2.3. Konfigurasi PHP

Kami menggunakan **[JENIS PHP: mod_php / php-fpm / lsphp]** untuk mengintegrasikan PHP dengan *Web Server*.

* **Instalasi PHP:**
    ```bash
    # [Tuliskan perintah instalasi PHP dan modul yang dibutuhkan]
    sudo apt install php-fpm php-mysql
    ```
* **Integrasi:**
    [Jelaskan langkah-langkah integrasi].

#### 2.4. Implementasi SSL (HTTPS)

Untuk mengaktifkan akses HTTPS, kami membuat *self-signed certificate*.

1.  Membuat direktori untuk *certificate*.
2.  Membuat *Key* dan *Certificate* menggunakan OpenSSL.
3.  Memodifikasi konfigurasi *Web Server* untuk menggunakan port **443** dan menunjuk ke *certificate* yang telah dibuat.

---

### 3. Analisis Web Server

Berdasarkan pengalaman kami dalam proyek ini, berikut adalah analisis kelebihan dan kekurangan dari *Web Server* yang kami gunakan:

| Aspek | Kelebihan ([NAMA WEB SERVER]) | Kekurangan ([NAMA WEB SERVER]) |
| :--- | :--- | :--- |
| **Performa & Kecepatan** | [Tuliskan kelebihannya. Contoh: Mampu menangani banyak koneksi bersamaan (Nginx).] | [Tuliskan kekurangannya. Contoh: Kurang efisien dalam melayani konten statis (Apache).] |
| **Kemudahan Konfigurasi**| [Tuliskan kelebihannya. Contoh: Konfigurasi yang terpusat dan modular (Apache).] | [Tuliskan kekurangannya. Contoh: Kurva belajar yang lebih curam karena sintaks baru (Nginx).] |
| **Fitur & Modularitas** | [Tuliskan kelebihannya.] | [Tuliskan kekurangannya.] |

---

### 4. Refleksi Proyek: Kesan dan Kendala

#### 4.1. Kesan Selama Proses Pengerjaan

[Tuliskan kesan anggota kelompok, misalnya: "Kami sangat senang karena proyek ini memberikan pemahaman langsung tentang proses deployment server yang sesungguhnya. Proses kolaborasi di GitHub juga mengajarkan pentingnya version control."]

#### 4.2. Kendala dan Solusi yang Diterapkan

| Kendala yang Kalian Hadapi | Solusi yang Ditemukan |
| :--- | :--- |
| [Contoh: Kesulitan mengintegrasikan PHP-FPM dengan Nginx.] | [Contoh: Kami mencari referensi dokumentasi resmi Nginx dan memastikan socket file PHP-FPM memiliki izin yang benar.] |
| [Tuliskan kendala teknis atau kolaborasi lain yang Kalian hadapi.] | [Jelaskan solusi spesifik Kalian.] |

---

### 5. Dokumentasi Video Pengerjaan

Seluruh proses pengerjaan telah direkam dan diunggah ke YouTube.

**Link Video YouTube:**

[![Thumbnail Video Pengerjaan](https://img.youtube.com/vi/**[ID_VIDEO_YOUTUBE_KALIAN]**/0.jpg)](**[LINK_LENGKAP_VIDEO_YOUTUBE_KALIAN]**)

**PETUNJUK:** Ganti semua teks di dalam tanda kurung siku `[ ... ]` dengan informasi proyek yang relevan.
