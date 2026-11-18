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
### 3. Menampilkan Data / Read (index.php)
Membuat file utama untuk menampilkan seluruh data barang dari database ke dalam bentuk tabel HTML
lengkap dengan styling CSS dan tombol aksi (Ubah & Hapus).

### 4. Menambah Data / Create (tambah.php)
Membuat form input data baru beserta fitur upload file gambar produk yang akan disimpan ke dalam
folder gambar/ dan datanya dimasukkan ke tabel data_barang.

### 5. Mengubah Data / Update (ubah.php)
Membuat form edit data berdasarkan id_barang untuk memperbarui informasi produk yang sudah ada di database.

### 6. Menghapus Data / Delete (hapus.php)
Membuat fungsi penghapusan data berdasarkan parameter id_barang yang diklik dari halaman utama.

