
### 27. Menghapus Primary Key
Menghapus primary key dari suatu tabel.
```sql
ALTER TABLE nama_tabel DROP PRIMARY KEY;
```

### 28. Menambahkan Foreign Key
Menambahkan foreign key untuk menghubungkan tabel.
```sql
ALTER TABLE anak ADD CONSTRAINT fk_parent FOREIGN KEY (id_parent) REFERENCES parent(id);
```

### 29. Menghapus Foreign Key
Menghapus foreign key yang telah dibuat sebelumnya.
```sql
ALTER TABLE anak DROP FOREIGN KEY fk_parent;
```

### 30. Membuat View
Membuat tampilan virtual dari data tabel tertentu.
```sql
CREATE VIEW view_nama AS
SELECT nama, usia FROM nama_tabel WHERE usia > 20;
```

### 31. Menghapus View
Menghapus tampilan (view) dari database.
```sql
DROP VIEW view_nama;
```

### 32. Menggunakan JOIN
Menghubungkan dua tabel berdasarkan kondisi tertentu.
```sql
SELECT a.id, a.nama, b.alamat 
FROM nama_tabel a
INNER JOIN alamat_tabel b ON a.id = b.id_user;
```

### 33. Menggunakan Transaksi
Menggunakan transaksi untuk memastikan perubahan data bersifat atomik.
```sql
START TRANSACTION;
INSERT INTO nama_tabel (nama, usia) VALUES ('Ali', 30);
SAVEPOINT sp1;
ROLLBACK TO sp1;
COMMIT;
```

