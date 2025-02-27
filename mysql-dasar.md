# Belajar MySQL dengan XAMPP (LAMPP di Linux)

MySQL adalah sistem manajemen basis data relasional (RDBMS) yang digunakan untuk mengelola dan mengakses data secara efisien. XAMPP (atau LAMPP di Linux) adalah paket perangkat lunak yang memudahkan instalasi MySQL bersama Apache dan PHP.

## Menjalankan dan Menghentikan MySQL di XAMPP

Untuk menjalankan MySQL menggunakan XAMPP di Linux, gunakan perintah berikut:

```sh
sudo /opt/lampp/lampp start
```

Untuk menghentikan MySQL:

```sh
sudo /opt/lampp/lampp stop
```

## Masuk ke MySQL/MariaDB

Untuk masuk ke MySQL/MariaDB sebagai pengguna root, gunakan perintah berikut:

```sh
/opt/lampp/bin/mysql -u root -p
```

---

## Perintah Dasar MySQL

Bagian ini mencakup perintah dasar yang sering digunakan dalam MySQL untuk membuat dan mengelola database serta tabel.

### 1. Melihat Daftar Database
Menampilkan daftar database yang tersedia dalam server MySQL.
```sql
SHOW DATABASES;
```

### 2. Membuat Database Baru
Membuat database baru dengan nama tertentu.
```sql
CREATE DATABASE nama_database;
```

### 3. Menggunakan Database
Memilih database yang ingin digunakan.
```sql
USE nama_database;
```

### 4. Melihat Daftar Tabel dalam Database
Menampilkan semua tabel yang ada dalam database yang sedang digunakan.
```sql
SHOW TABLES;
```

### 5. Membuat Tabel Baru
Membuat tabel baru dengan kolom tertentu.
```sql
CREATE TABLE nama_tabel (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nama VARCHAR(100) NOT NULL,
    usia INT NOT NULL
);
```

### 6. Melihat Struktur Tabel
Menampilkan struktur tabel, termasuk kolom dan tipe datanya.
```sql
DESC nama_tabel;
```
atau
```sql
SHOW COLUMNS FROM nama_tabel;
```

### 7. Menambahkan Data ke dalam Tabel
Menambahkan data baru ke dalam tabel yang telah dibuat.
```sql
INSERT INTO nama_tabel (nama, usia) VALUES ('Yunus', 23);
```

### 8. Melihat Seluruh Data dalam Tabel
Menampilkan seluruh data yang ada dalam tabel.
```sql
SELECT * FROM nama_tabel;
```

### 9. Memperbarui Data dalam Tabel
Mengubah data yang sudah ada berdasarkan kondisi tertentu.
```sql
UPDATE nama_tabel SET usia = 24 WHERE id = 1;
```

### 10. Menghapus Data dari Tabel
Menghapus data tertentu dari tabel berdasarkan kondisi.
```sql
DELETE FROM nama_tabel WHERE id = 1;
```

### 11. Menghapus Tabel
Menghapus tabel beserta seluruh isinya.
```sql
DROP TABLE nama_tabel;
```

### 12. Menghapus Database
Menghapus database beserta seluruh tabelnya.
```sql
DROP DATABASE nama_database;
```
