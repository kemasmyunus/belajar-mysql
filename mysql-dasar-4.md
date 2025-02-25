Mengubah Nama Tabel
sql
Salin
Edit
ALTER TABLE nama_tabel RENAME TO nama_tabel_baru;
Mengubah Nama Kolom
sql
Salin
Edit
ALTER TABLE nama_tabel CHANGE COLUMN kolom_lama kolom_baru VARCHAR(255);
Menambahkan Indeks ke Kolom
sql
Salin
Edit
CREATE INDEX idx_nama ON nama_tabel(nama






Anda bilang:
lanjutkan
ChatGPT bilang:
Menghapus Indeks dari Kolom
sql
Salin
Edit
DROP INDEX idx_nama ON nama_tabel;
Menambahkan Primary Key
sql
Salin
Edit
ALTER TABLE nama_tabel ADD PRIMARY KEY (nama_kolom);
Menghapus Primary Key
sql
Salin
Edit
ALTER TABLE nama_tabel DROP PRIMARY KEY;
Menambahkan Foreign Key
sql
Salin
Edit
ALTER TABLE anak ADD CONSTRAINT fk_parent FOREIGN KEY (id_parent) REFERENCES parent(id);
Menghapus Foreign Key
sql
Salin
Edit
ALTER TABLE anak DROP FOREIGN KEY fk_parent;
Melihat Struktur Tabel
sql
Salin
Edit
DESC nama_tabel;
atau

sql
Salin
Edit
SHOW COLUMNS FROM nama_tabel;
Melihat Semua Tabel dalam Database
sql
Salin
Edit
SHOW TABLES;






