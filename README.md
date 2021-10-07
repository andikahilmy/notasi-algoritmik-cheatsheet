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

### Tipe Data Struct

Contoh:

```
type Time: 	  < hours: integer[0..23], 		{ 0 ≤ hours ≤ 23 }
				minutes: integer[0..59], 	{ 0 ≤ minutes ≤ 59 }
				seconds: integer[0..59] > 	{ 0 ≤ seconds ≤ 59 }
```

### Operator

* Tambah: `+`
* Kurang: `-`
* Kali: `*`
* Bagi: `/`
* Assignment `←`
* Input: `input()`
* Output: `output()`

Catatan: Output bisa mengandung new line atau tidak, suka-suka aja
