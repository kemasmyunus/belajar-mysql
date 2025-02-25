# Perintah Lanjutan MySQL

## 22. Mengubah Nama Tabel
```sql
ALTER TABLE nama_tabel RENAME TO nama_tabel_baru;
```

## 23. Mengubah Nama Kolom
```sql
ALTER TABLE nama_tabel CHANGE COLUMN kolom_lama kolom_baru VARCHAR(255);
```

## 24. Menambahkan Indeks ke Kolom
```sql
CREATE INDEX idx_nama ON nama_tabel(nama_kolom);
```

## 25. Menghapus Indeks dari Kolom
```sql
DROP INDEX idx_nama ON nama_tabel;
```

## 26. Menambahkan Primary Key
```sql
ALTER TABLE nama_tabel ADD PRIMARY KEY (nama_kolom);
```

## 27. Menghapus Primary Key
```sql
ALTER TABLE nama_tabel DROP PRIMARY KEY;
```

## 28. Menambahkan Foreign Key
```sql
ALTER TABLE anak ADD CONSTRAINT fk_parent FOREIGN KEY (id_parent) REFERENCES parent(id);
```

## 29. Menghapus Foreign Key
```sql
ALTER TABLE anak DROP FOREIGN KEY fk_parent;
```

## 30. Melihat Struktur Tabel
```sql
DESC nama_tabel;
```
atau
```sql
SHOW COLUMNS FROM nama_tabel;
```

## 31. Melihat Semua Tabel dalam Database
```sql
SHOW TABLES;
```
