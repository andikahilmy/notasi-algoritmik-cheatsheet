# Notasi Algoritmik CheatSheet

Kitab lengkap notasi algoritmik --kalo ada yang kurang bisa tambahin aja

Daftar isi:

* Struktur umum


### Struktur Umum

```
Program NamaProgram
{ Spesifikasi Program: Tuliskan di sini }

KAMUS
{ Deklarasi variabel }
	a, b: integer

ALGORITMA
input(a)
input(b)
a ← a + b
output(a)
```

### Tipe Data Umum

* `integer`
* `real`
* `character`
* `array [firstElmt..lastElmt] of datatype`

### Tipe Data Struct

```
type Struct:	< data1: integer,	{ integer dibolehkan }
		data2: integer[0..69],	{ integer dengan range 0..69 }
		data3: real,	{ tipe data real juga dibolehkan }
		data4: array[0..9] of character >	{ karakter/string juga dibolehkan }
```
Contoh:

```
type Time:    < hours: integer[0..23], 		{ 0 ≤ hours ≤ 23 }
		minutes: integer[0..59], 	{ 0 ≤ minutes ≤ 59 }
		seconds: integer[0..59] > 	{ 0 ≤ seconds ≤ 59 }
```

### Operator

* Tambah: `+`
* Kurang: `-`
* Kali: `*`
* Bagi: `/`
* Lebih besar dari: `>`
* Lebih kecil dari: `<`
* Tidak sama dengan: `!=` atau `≠`
* Tidak kurang dari: `>=` atau `≥`
* Tidak lebih dari: `<=` atau `≤`
* Sama dengan: `=`
* Assignment `←` atau `<-`
* Input: `input()`
* Output: `output()`

Catatan: Output bisa mengandung new line atau tidak, suka-suka aja
