# Notasi Algoritmik CheatSheet

Kitab lengkap notasi algoritmik --kalo ada yang kurang bisa tambahin aja

Daftar isi:

* Notasi Algoritmik Umum

## Notasi Algoritmik Umum

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
* `boolean`
* `array [firstElmt..lastElmt] of datatype`

### Operator

* Tambah: `+`
* Kurang: `-`
* Kali: `*`
* Bagi: `/`
* Hasil bagi: `div`
* Modulo: `mod`
* Lebih besar dari: `>`
* Lebih kecil dari: `<`
* Tidak sama dengan: `!=` atau `≠` (U+2260)
* Tidak kurang dari: `>=` atau `≥` (U+2265)
* Tidak lebih dari: `<=` atau `≤` (U+2264)
* Sama dengan: `=`
* Boolean and: `and`
* Boolean or: `or`
* Boolean not: `not`
* Boolean xor: `xor`
* Assignment: `←` (U+2190) atau `<-`
* Return: `→`(U+2192) atau `->`
* Input: `input()`
* Output: `output()`

Catatan

* `div` hanya berlaku untuk dua operan integer
* Output bisa mengandung new line atau tidak, suka-suka aja
* Return dan `not` operator adalah operator uner
* Bedakan antara `x < -2` dengan `x <- 2`

### Tipe Data Struct

```
type Struct:    < data1: integer,					{ integer dibolehkan }
                  data2: integer[0..69],			{ integer dengan range 0..69 }
                  data3: real,						{ tipe data real juga dibolehkan }
                  data4: array[0..9] of character >	{ karakter/string juga dibolehkan }
```

Cara akses variabel: `varName.data1`, `varName.data2`, dsb.

Contoh:

```
type Time:    < hours: integer[0..23], 		{ 0 ≤ hours ≤ 23 }
                minutes: integer[0..59], 	{ 0 ≤ minutes ≤ 59 }
                seconds: integer[0..59] > 	{ 0 ≤ seconds ≤ 59 }
```

### Ekspresi

Sekumpulan rumus perhitungan dari operan dan operator.

Contoh: `2 + 8 * (x mod 4)`

### Nama Variabel dan konstanta

Berikut ini adalah nama variabel/konstanta yang dibolehkan

* `varName`
* `VarName`
* `varname`
* `Var1`
* `PI` (khusus konstanta, contoh: `IDX_UNDEF`, `VAL_UNDEF`)

Nama variabel yang tidak dibolehkan

* `1cak`
* `*GWS`
* `kereta-api`

## Fungsi dan Prosedur

### Fungsi

Struktur umum
```
function NamaFungsi(param1: type1, param2: type2, parametc: typeetc) → typehasil
{ Mengembalikan fafifu dari wasweswos }

KAMUS LOKAL
{ Nama variabel lokal : tipe data }

ALGORITMA
{ Deretan instruksi }
    
    → hasil
```

## Loop

### For/Traversal

Beberapa bentuk yang dibolehkan:
```
i traversal (0..10)
    { langkah 1 }
    { langkah 2 }
    { langkah 3 dan seterusnya }
```

```
i traversal
```



