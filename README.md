# Laporan Praktikum 8: PHP dan Database MySQL
Repository ini dibuat untuk memenuhi tugas **Praktikum 8: PHP dan Database MySQL** pada mata kuliah Pemrograman Web.

## 🛠️ Langkah-Langkah Praktikum

### 1. Persiapan Lingkungan & Database
* **XAMPP Server**: Menyalakan modul Apache dan MySQL pada XAMPP Control Panel.
* **Database MySQL**: Membuat database baru dengan nama `latihan1` melalui phpMyAdmin.
* **Tabel `data_barang`**: Membuat tabel dengan struktur field sebagai berikut[cite: 2]:
  * `id_barang` (INT, 10) - Primary Key, Auto Increment[cite: 2]
  * `kategori` (VARCHAR, 30)[cite: 2]
  * `nama` (VARCHAR, 30 / 50)[cite: 2]
  * `gambar` (VARCHAR, 100)[cite: 2]
  * `harga_beli` (DECIMAL/INT, 8/10)[cite: 2]
  * `harga_jual` (DECIMAL/INT, 8/10)[cite: 2]
  * `stok` (INT, 4)[cite: 2]

---
<img width="500" height="322" alt="Cuplikan layar 2026-11-18 113048" src="https://github.com/user-attachments/assets/3425e863-3560-48f4-a19a-774e1dfa7fda" />
<img width="768" height="437" alt="Cuplikan layar 2026-11-18 113158" src="https://github.com/user-attachments/assets/b02165d9-a644-42a7-b453-1030cb482d02" />



### 2. Membuat Koneksi Database (`koneksi.php`)
Membuat file koneksi untuk menghubungkan PHP dengan database MySQL menggunakan ekstensi `mysqli`.
```php
<?php
$host = "localhost";
$user = "root";
$pass = "";
$db = "latihan1";
$conn = mysqli_connect($host,$user, $pass,$db);
if ($conn == false) {
    echo "Koneksi ke server gagal.";
    die();
}
?>

### 3. Menampilkan Data / Read (`index.php`)
Membuat file utama untuk menampilkan seluruh data barang dari database ke dalam bentuk tabel HTML lengkap dengan styling CSS dan tombol aksi (Ubah & Hapus).

---
<img width="836" height="472" alt="Cuplikan layar 2026-11-18 120118" src="https://github.com/user-attachments/assets/bf3c840c-6800-46e9-b9ea-9780d5a05068" />

### 4. Menambah Data / Create (`tambah.php`)
Membuat form input data baru beserta fitur upload file gambar produk yang akan disimpan ke dalam folder `gambar/` dan datanya dimasukkan ke tabel `data_barang`.

---
<img width="839" height="533" alt="Cuplikan layar 2026-11-18 113248" src="https://github.com/user-attachments/assets/7d955e65-d9cc-4021-8b53-be59cb521be5" />
<img width="834" height="532" alt="Cuplikan layar 2026-11-18 113231" src="https://github.com/user-attachments/assets/cc5cb5f9-9f74-4c82-b005-ebf2924095fd" />

### 5. Mengubah Data / Update (`ubah.php`)
Membuat form edit data berdasarkan `id_barang` untuk memperbarui informasi produk yang sudah ada di database.

---

### 6. Menghapus Data / Delete (`hapus.php`)
Membuat fungsi penghapusan data berdasarkan parameter `id_barang` yang diklik dari halaman utama.
<img width="859" height="457" alt="Cuplikan layar 2026-11-18 120527" src="https://github.com/user-attachments/assets/14b9af5d-e0a6-42dd-9297-cf0fe0680a45" />
<img width="841" height="470" alt="Cuplikan layar 2026-11-18 120300" src="https://github.com/user-attachments/assets/0b079856-6b8f-4db5-bb7d-50267c636cbb" />

