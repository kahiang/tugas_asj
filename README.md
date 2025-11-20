# 📄 TEMPLATE LAPORAN PROYEK: PENGEMBANGAN WEB SERVER DAN APLIKASI SEDERHANA

**Proyek:** [JUDUL PROYEK KELOMPOK]

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
    # [Tuliskan perintah instalasi Web Server kalian, contoh: sudo apt install nginx -y]
    ```
* **Konfigurasi Virtual Host/Server Block:**
    [Jelaskan secara singkat penyesuaian konfigurasi yang dilakukan pada file utama (`/etc/apache2/sites-available/000-default.conf` atau `/etc/nginx/sites-available/default`)].

#### 2.3. Konfigurasi PHP

Kami menggunakan **[JENIS PHP: mod_php / php-fpm / lsphp]** untuk mengintegrasikan PHP dengan *Web Server*.

* **Instalasi PHP:**
    ```bash
    # [Tuliskan perintah instalasi PHP dan modul yang dibutuhkan]
    sudo apt install php-fpm php-mysql
    ```
* **Integrasi:**
    [Jelaskan langkah-langkah integrasi (misalnya, mengaktifkan `proxy_pass` ke `php-fpm.sock` di Nginx, atau mengaktifkan `mod_php` di Apache)].

#### 2.4. Implementasi SSL (HTTPS)

Untuk mengaktifkan akses HTTPS, kami membuat *self-signed certificate*.

1.  Membuat direktori untuk *certificate*.
    ```bash
    # [Tuliskan perintah membuat direktori]
    ```
2.  Membuat *Key* dan *Certificate* menggunakan OpenSSL.
    ```bash
    # [Tuliskan perintah OpenSSL yang digunakan]
    ```
3.  Memodifikasi konfigurasi *Web Server* untuk menggunakan port **443** dan menunjuk ke *certificate* yang telah dibuat.

---

### 3. Dokumentasi Konten Website

Seluruh *source code* (Halaman Utama dan Halaman Profil) yang berada di *document root* server (`/var/www/html/`) telah disalin dan di-*commit* ke dalam folder `/html` di *repository* GitHub ini.

| Konten Web | Keterangan |
| :--- | :--- |
| `html/index.[php/html]` | Halaman utama kelompok. |
| `html/[nama_anggota]` | Folder yang berisi halaman profil masing-masing anggota. |
| Bahasa yang digunakan | HTML, CSS, dan PHP. |

---

### 4. Dokumentasi Video Pengerjaan

Seluruh proses pengerjaan, mulai dari penyiapan VM hingga pengujian akses HTTPS dan *commit* kode, telah direkam dan diunggah ke YouTube.

**Link Video YouTube:**

[![Thumbnail Video Pengerjaan](https://img.youtube.com/vi/1-qlNtQS1OA/0.jpg)](https://www.youtube.com/watch?v=1-qlNtQS1OA)

**PETUNJUK:** Ganti `[ID_VIDEO_YOUTUBE]` dan `[LINK_LENGKAP_VIDEO_YOUTUBE]` dengan informasi video kelompok kalian.
