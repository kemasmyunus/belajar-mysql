## Perintah Lanjutan MySQL

Bagian ini mencakup perintah yang lebih kompleks untuk mengelola struktur database, pengguna, serta melakukan backup dan transaksi data.

### 13. Menambahkan Kolom Baru ke Tabel
Menambahkan kolom baru ke dalam tabel yang sudah ada.
```sql
ALTER TABLE nama_tabel ADD COLUMN alamat VARCHAR(255);
```

### 14. Mengubah Tipe Data Kolom
Mengubah tipe data dari suatu kolom dalam tabel.
```sql
ALTER TABLE nama_tabel MODIFY COLUMN usia SMALLINT;
```

### 15. Menghapus Kolom dari Tabel
Menghapus kolom tertentu dari tabel.
```sql
ALTER TABLE nama_tabel DROP COLUMN alamat;
```

### 16. Mengubah Nama Tabel
Mengubah nama tabel menjadi nama baru.
```sql
ALTER TABLE nama_tabel RENAME TO nama_tabel_baru;
```

### 17. Mengubah Nama Kolom
Mengubah nama suatu kolom dalam tabel.
```sql
ALTER TABLE nama_tabel CHANGE COLUMN kolom_lama kolom_baru VARCHAR(255);
```

### 18. Membuat Pengguna Baru
Membuat akun pengguna baru dalam MySQL.
```sql
CREATE USER 'userbaru'@'localhost' IDENTIFIED BY 'password123';
```

### 19. Memberikan Hak Akses ke Pengguna
Memberikan izin akses kepada pengguna tertentu terhadap database.
```sql
GRANT ALL PRIVILEGES ON nama_database.* TO 'userbaru'@'localhost';
```

### 20. Menampilkan Hak Akses Pengguna
Menampilkan hak akses yang dimiliki oleh seorang pengguna.
```sql
SHOW GRANTS FOR 'userbaru'@'localhost';
```

### 21. Menghapus Pengguna
Menghapus akun pengguna dari MySQL.
```sql
DROP USER 'userbaru'@'localhost';
```
