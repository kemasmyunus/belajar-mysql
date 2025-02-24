# Belajar MySQL dengan XAMPP (LAMPP di Linux)

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

### 1. Melihat Daftar Database
```sql
SHOW DATABASES;
```

### 2. Membuat Database Baru
```sql
CREATE DATABASE nama_database;
```

### 3. Menggunakan Database
```sql
USE nama_database;
```

### 4. Melihat Daftar Tabel dalam Database
```sql
SHOW TABLES;
```

### 5. Membuat Tabel Baru
```sql
CREATE TABLE nama_tabel (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nama VARCHAR(100) NOT NULL,
    usia INT NOT NULL
);
```

### 6. Melihat Struktur Tabel
```sql
DESC nama_tabel;
```

### 7. Menambahkan Data ke dalam Tabel
```sql
INSERT INTO nama_tabel (nama, usia) VALUES ('Yunus', 23);
```

### 8. Melihat Seluruh Data dalam Tabel
```sql
SELECT * FROM nama_tabel;
```

### 9. Memperbarui Data dalam Tabel
```sql
UPDATE nama_tabel SET usia = 24 WHERE id = 1;
```

### 10. Menghapus Data dari Tabel
```sql
DELETE FROM nama_tabel WHERE id = 1;
```

### 11. Menghapus Tabel
```sql
DROP TABLE nama_tabel;
```

### 12. Menghapus Database
```sql
DROP DATABASE nama_database;
```
