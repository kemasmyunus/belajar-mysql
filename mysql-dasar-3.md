22. Membuat Index pada Tabel

CREATE INDEX idx_nama ON nama_tabel(nama);

23. Menghapus Index dari Tabel

DROP INDEX idx_nama ON nama_tabel;

24. Membuat View

CREATE VIEW view_nama AS
SELECT nama, usia FROM nama_tabel WHERE usia > 20;

25. Melihat Data dari View

SELECT * FROM view_nama;

26. Menghapus View

DROP VIEW view_nama;

27. Menggunakan JOIN (INNER JOIN)

SELECT a.id, a.nama, b.alamat 
FROM nama_tabel a
INNER JOIN alamat_tabel b ON a.id = b.id_user;

28. Menggunakan LEFT JOIN

SELECT a.id, a.nama, b.alamat 
FROM nama_tabel a
LEFT JOIN alamat_tabel b ON a.id = b.id_user;

29. Menggunakan RIGHT JOIN

SELECT a.id, a.nama, b.alamat 
FROM nama_tabel a
RIGHT JOIN alamat_tabel b ON a.id = b.id_user;

30. Membuat Stored Procedure

DELIMITER //
CREATE PROCEDURE tambah_pengguna(IN nama_pengguna VARCHAR(100), IN usia_pengguna INT)
BEGIN
    INSERT INTO nama_tabel(nama, usia) VALUES (nama_pengguna, usia_pengguna);
END //
DELIMITER ;

31. Menjalankan Stored Procedure

CALL tambah_pengguna('Ahmad', 25);

32. Menghapus Stored Procedure

DROP PROCEDURE tambah_pengguna;

33. Membuat Trigger

DELIMITER //
CREATE TRIGGER sebelum_insert
BEFORE INSERT ON nama_tabel
FOR EACH ROW
BEGIN
    SET NEW.nama = UPPER(NEW.nama);
END //
DELIMITER ;

34. Menghapus Trigger

DROP TRIGGER sebelum_insert;

35. Menggunakan Transaksi (Transaction)

START TRANSACTION;
INSERT INTO nama_tabel (nama, usia) VALUES ('Ali', 30);
SAVEPOINT sp1;
INSERT INTO nama_tabel (nama, usia) VALUES ('Budi', 28);
ROLLBACK TO sp1;
COMMIT;
