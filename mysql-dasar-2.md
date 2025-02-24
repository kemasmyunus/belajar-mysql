Perintah Lanjutan MySQL

13. Menambahkan Kolom Baru ke Tabel

ALTER TABLE nama_tabel ADD COLUMN alamat VARCHAR(255);

14. Mengubah Tipe Data Kolom

ALTER TABLE nama_tabel MODIFY COLUMN usia SMALLINT;

15. Menghapus Kolom dari Tabel

ALTER TABLE nama_tabel DROP COLUMN alamat;

16. Membuat Pengguna Baru

CREATE USER 'userbaru'@'localhost' IDENTIFIED BY 'password123';

17. Memberikan Hak Akses ke Pengguna

GRANT ALL PRIVILEGES ON nama_database.* TO 'userbaru'@'localhost';

18. Menampilkan Hak Akses Pengguna

SHOW GRANTS FOR 'userbaru'@'localhost';

19. Menghapus Pengguna

DROP USER 'userbaru'@'localhost';

20. Backup Database

mysqldump -u root -p nama_database > backup.sql

21. Restore Database dari Backup

mysql -u root -p nama_database < backup.sql

Dengan perintah lanjutan ini, Anda dapat lebih fleksibel dalam mengelola MySQL. Selamat belajar! 🚀

