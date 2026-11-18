# Laporan Praktikum 8: PHP dan Database MySQL
Repository ini dibuat untuk memenuhi tugas Praktikum 8: PHP dan Database MySQL pada mata kuliah Pemrograman Web.

## Langkah-Langkah Praktikum

### 1. Persiapan Lingkungan & Database
* XAMPP Server: Menyalakan modul Apache dan MySQL pada XAMPP Control Panel.
* Database MySQL: Membuat database baru dengan nama latihan1 melalui phpMyAdmin.
* Tabel data_barang: Membuat tabel dengan struktur field: id_barang, kategori, nama, gambar, harga_beli, harga_jual, dan stok.
<img width="500" height="322" alt="Cuplikan layar 2026-11-18 113048" src="https://github.com/user-attachments/assets/2daabcdf-67fa-4617-821d-3ddf2611e6c1" />
<img width="768" height="437" alt="Cuplikan layar 2026-11-18 113158" src="https://github.com/user-attachments/assets/79b32775-b355-4d0e-9ce5-fb71840d6c98" />

### 2. Membuat Koneksi Database (koneksi.php)
Membuat file koneksi untuk menghubungkan PHP dengan database MySQL menggunakan ekstensi mysqli.

### 3. Menampilkan Data / Read (index.php)
Membuat file utama untuk menampilkan seluruh data barang dari database ke dalam bentuk tabel HTML lengkap dengan styling CSS dan tombol aksi (Ubah & Hapus).
<img width="836" height="472" alt="Cuplikan layar 2026-11-18 120118" src="https://github.com/user-attachments/assets/a8810bb6-896a-4eb3-ad59-d2ad4190cc13" />

### 4. Menambah Data / Create (tambah.php)
Membuat form input data baru beserta fitur upload file gambar produk yang akan disimpan ke dalam folder gambar/ dan datanya dimasukkan ke tabel data_barang.
<img width="834" height="532" alt="Cuplikan layar 2026-11-18 113231" src="https://github.com/user-attachments/assets/dbc09782-ab3d-4497-bfb0-eaf7999666b8" />

### 5. Mengubah Data / Update (ubah.php)
Membuat file form edit data berdasarkan id_barang untuk memperbarui informasi produk yang sudah ada di database.
<img width="839" height="533" alt="Cuplikan layar 2026-11-18 113248" src="https://github.com/user-attachments/assets/1cb85c70-888e-487f-9d8c-2b5687b8fc76" />

### 6. Menghapus Data / Delete (hapus.php)
Membuat fungsi penghapusan data berdasarkan parameter id_barang yang diklik dari halaman utama.
<img width="841" height="470" alt="Cuplikan layar 2026-11-18 120300" src="https://github.com/user-attachments/assets/775df0ca-3a88-42ec-92f2-08f46b2c44ad" />
<img width="859" height="457" alt="Cuplikan layar 2026-11-18 120527" src="https://github.com/user-attachments/assets/e45ccc1a-09b4-4065-884c-bcee0c60f811" />

## Cara Menjalankan Program
1. Clone atau download repository ini.
2. Letakkan folder project ke dalam direktori root web server XAMPP (htdocs).
3. Import database latihan1 melalui phpMyAdmin.
4. Nyalakan Apache dan MySQL di XAMPP Control Panel.
5. Buka browser dan akses URL: http://localhost/Lab8Web/

