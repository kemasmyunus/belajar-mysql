
### 22. Backup Database
Membuat cadangan (backup) database ke dalam file SQL.
```sh
mysqldump -u root -p nama_database > backup.sql
```

### 23. Restore Database dari Backup
Mengembalikan database dari file backup SQL.
```sh
mysql -u root -p nama_database < backup.sql
```

### 24. Membuat Indeks pada Tabel
Membuat indeks pada kolom tertentu untuk mempercepat pencarian data.
```sql
CREATE INDEX idx_nama ON nama_tabel(nama);
```

### 25. Menghapus Indeks dari Tabel
Menghapus indeks yang telah dibuat pada tabel.
```sql
DROP INDEX idx_nama ON nama_tabel;
```

### 26. Menambahkan Primary Key
Menjadikan suatu kolom sebagai primary key.
```sql
ALTER TABLE nama_tabel ADD PRIMARY KEY (nama_kolom);
```
