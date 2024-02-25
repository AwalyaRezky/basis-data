# AND
## Struktur Query
```mysql
SELECT kolom1,kolom2 FROM [nama_tabel] WHERE kolom1="nilai1" AND kolom2="nilai2";
```
## Contoh Query
```MYSQL
SELECT warna,pemilik FROM mobil WHERE warna="HITAM" AND pemilik="REZKY";
```
## Hasil
![[Screenshot 2024-02-20 141411.png|500]]

## Analisis

## Kesimpulan


# OR
## Struktur Query
```MYSQL
 SELECT kolom1,kolom2 FROM [nama_tabel] WHERE kolom1="nilai1" OR kolom2="nilai2";
```
## Contoh Query
```MYSQL
 SELECT warna,pemilik FROM mobil WHERE warna="HITAM" OR pemilik="REZKY";
```
## Hasil
![[lanjutan (2).png|500]]

## Analisis

## Kesimpulan

# BETWEEN
## Struktur Query
```MYSQL
 SELECT * FROM [nama_tabel] WHERE kolom1 BETWEEN nilai1 AND nilai2;
```
## Contoh Query
```mysql
 SELECT * FROM mobil WHERE harga_rental BETWEEN 50000 AND 100000;
```
## Hasil
![[lanjutan (3).png|500]]

## Analisis
## Kesimpulan
# NOT BETWEEN
## Struktur Query
```MYSQL
 SELECT * FROM [nama_tabel] WHERE kolom1 NOT BETWEEN nilai1 AND nilai2;
```
## Contoh Query
```MYSQL
 SELECT * FROM mobil WHERE harga_rental NOT BETWEEN 100000 AND 150000;
```
## Hasil
![[not between.png|500]]

## Analisis
## Kesimpulan
# <=
## Struktur Query
```mysql
 SELECT * FROM [nama_tabel] WHERE kolom1 <= nilai1;
```
## Contoh Query
```mysql
 SELECT * FROM mobil WHERE harga_rental <= 100000;
```
## Hasil
![[lebih kecil.png|500]]

## Analisis
## Kesimpulan
# >=
## Struktur Query
```mysql
SELECT * FROM [nama_tabel] WHERE kolom1 >= nilai1;
```
## Contoh Query
```mysql
SELECT * FROM mobil WHERE harga_rental >= 100000;
```
## Hasil
![[lebih besar.png|500]]

## Analisis
## Kesimpulan
# <> atau !=
## Struktur Query
```mysql
SELECT * FROM [nama_tabel] WHERE kolom1 <> nilai1;

SELECT * FROM [nama_tabel] WHERE kolom1 != nilai1;
```
## Contoh Query
```mysql
SELECT * FROM mobil WHERE harga_rental <> 100000;

SELECT * FROM mobil WHERE harga_rental != 50000;
```
## Hasil
![[tidak sama dengan.png|500]]

![[tdk sma dgn.png|500]]


## Analisis

## Kesimpulan

# Tantangan login
## IN
### Struktur Querry
```mysql
SELECT * FROM [nama_tabel] WHERE [nama_kolom] IN("nilai1","nilai2");
```
### Contoh Query
```MYSQL
 SELECT * FROM mobil WHERE warna IN("Silver","Merah");
```
### Hasil
![[IN.png|500]]

### Analisis

### Kesimpulan
## IN + AND
### Struktur Query
```mysql
  SELECT * FROM [nama_tabel]
-> WHERE [nama_kolom1] IN("nilai1","nilai2")
-> AND [nama_kolom2] = nilai;
```
### Contoh Query
```MYSQL
  SELECT * FROM mobil
-> WHERE warna IN("Silver","Merah")
-> AND harga_rental = 50000;
```
### Hasil
![[in and.png|500]]


### Analisis

### Kesimpulan
## IN + OR
### Struktur Query
```mysql
SELECT * FROM [nama_tabel]
-> WHERE [nama_kolom1] IN ('nilai1','nilai2')
-> OR [nama_kolom2] = nilai1;
```
### Contoh Query
```MYSQL
SELECT * FROM mobil
-> WHERE warna IN ('Hitam','Silver')
-> OR harga_rental = 150000;
```
### Hasil
![[in or.png|500]]

### Analisis

### Kesimpulan
## IN + AND + OPERATOR
### Struktur Query
```mysql
 SELECT * FROM [nama_tabel]
-> WHERE [nama_kolom1] IN ('nilai1','nilai2')
-> AND [nama_kolom2] > nilai1;

 SELECT * FROM [nama_tabel]
-> WHERE [nama_kolom1] IN ('nilai1','nilai2')
-> AND [nama_kolom2] < nilai1![[tntngan lbih kcil.png]];
```
### Contoh Query
```MYSQL
 SELECT * FROM mobil
-> WHERE warna IN ('Hitam','Silver')
-> AND harga_rental > 50000;

 SELECT * FROM mobil
-> WHERE warna IN ('Hitam','Silver')
-> AND harga_rental < 150000;
```
### Hasil
![[tntngan lebih besar.png|500]]

![[tntngan lbih kcil.png|500]]


### Analisis

### Kesimpulan


