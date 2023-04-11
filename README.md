# praktikum
# Tugas-Basis-Data

1. Buat sebuah database dengan nama latihan2!
``` 
CREATE DATABASE latihan1;
```
![Gambar1](Gambar/barbar1.png)
![Gambar1](Gambar/barbar2.png)

2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam
database latihan1!
```
CREATE TABLE siswa (nama VARCHAR(100), alamat TEXT);
```
![Gambar1](Gambar/barbar3.png)


3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom
terakhir!
```
ALTER TABLE siswa ADD COLUMN keterangan varchar(15) AFTER alamat;
```
![Gambar1](Gambar/barbar4.png)

4. Tambahkan kolom id (int 11) di awal (sebagai kolom pertama)!
```
ALTER TABLE siswa ADD COLUMN id int(11) First;
```
![Gambar1](Gambar/barbar5.png)

5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah
kolom alamat!
```
ALTER TABLE siswa ADD COLUMN phone varchar(15) after alamat;
```
![Gambar1](Gambar/barbar6.png)


6. Ubah tipe data kolom id menjadi char(11)!
```
ALTER TABLE siswa MODIFY COLUMN id VARCHAR(11);
```
![Gambar1](Gambar/barbar7.png)


7. Ubah nama kolom phone menjadi hp (varchar 20)!
```
ALTER TABLE siswa CHANGE COLUMN phone hp varchar(20);
```
![Gambar1](Gambar/barbar8.png)

8. Tambahkan kolom email setelah kolom hp
```
ALTER TABLE siswa ADD COLUMN email text after hp;
```
![Gambar1](Gambar/barbar9.png)


9. Hapus kolom keterangan dari tabel!
```
alter table siswa drop keterangan;
```
![Gambar1](Gambar/barbar10.png)


10. Ganti nama tabel menjadi data_mahasiswa!
```
alter table siswa rename data_mahasiswa;
```
![Gambar1](Gambar/barbar11.png)

11. Ganti nama field id menjadi nim!
```
ALTER TABLE data_mahasiswa CHANGE COLUMN id nim varchar(11);
```
![Gambar1](Gambar/barbar12.png)


12. Jadikan nim sebagai PRIMARY KEY!
```
ALTER TABLE data_mahasiswa ADD PRIMARY KEY(nim);
```
![Gambar1](Gambar/barbar13.png)


13. Jadikan kolom email sebagai UNIQUE KEY
```
ALTER TABLE data_mahasiswa ADD CONSTRAINT email unique KEY(email);
```
![Gambar1](Gambar/barbar14.png)


14. Hasil akhir

![Gambar1](Gambar/barbar15.png)


# Evaluasi dan pertanyaan
1. Apa maksud dari int (11)?
```
int (11) nunjukkan bahwa kolom memiliki tipe data bilangan bulat (integer) dengan ukuran 11 digit 
```

2. Ketika kita melihat struktur tabel dengan perintah desc, ada kolom Null yang
berisi Yes dan No. Apa maksudnya ?
```
Jika kolom "Null" adalah "YES", itu berarti kolom tersebut diizinkan untuk memiliki nilai NULL.

Jika kolom "Null" adalah "NO", maka kolom tersebut tidak diizinkan untuk memiliki nilai NULL
```
