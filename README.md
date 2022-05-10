# Notasi Algoritmik CheatSheet

Kitab lengkap notasi algoritmik --kalo ada yang kurang bisa tambahin aja

## DISCLAIMER: Pemilik Repositori tidak akan bertanggung jawab untuk segala tindak kecurangan pada ujian (closed book) yang melibatkan repositori ini!!!

Daftar isi:

* [Notasi Algoritmik Umum](#notasi-algoritmik-umum)
  * [Struktur Umum](#struktur-umum)
  * [Tipe Data Umum](#tipe-data-umum)
  * [Operator](#operator)
  * [Tipe Data Bentukan](#tipe-data-bentukan)
  * [Ekspresi](#ekspresi)
  * [Nama Variabel dan Konstanta](#nama-variabel-dan-konstanta)
  * [Array](#array)
* [Fungsi dan Prosedur](#fungsi-dan-prosedur)
  * [Fungsi](#fungsi)
  * [Prosedur](#prosedur)
* [Loop](#loop)
  * [Repeat N Times](#repeat-n-times)
  * [Repeat-Until](#repeat-until)
  * [While](#while)
  * [Iterate-Stop](#iterate-stop)
  * [For/Traversal](#fortraversal)

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

### Tipe Data Bentukan

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

### Nama Variabel dan Konstanta

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

### Array

```
NamaArray : array [valMin..valMax] of datatype
```

Keterangan:
* `NamaArray` bisa apa saja
* `valMin` biasanya adalah `0`, `valMax` terserah
* `valMin` dan `valMax` harus merupakan tipe integer
* `datatype` bebas, bisa data bentukan/struct

Contoh:
```
arrayInt : array[0..8] of integer
arrayJam : array[0..59] of Jam
```

Cara akses: `NamaArray[idx]` dengan `idx` harus di dalam range definisi array tersebut

## Fungsi dan Prosedur

### Fungsi

Struktur umum
```
function NamaFungsi(input param1: type1, input param2: type2, input parametc: typeetc) → output typehasil
{ Mengembalikan fafifu dari wasweswos }

KAMUS LOKAL
{ Nama variabel lokal : tipe data }

ALGORITMA
{ Deretan instruksi }
    
    → hasil
```

Pemanggilan
```
NamaFungsi(param1, param2, parametc)
```

Catatan: jumlah parameter bebas, bisa juga tanpa parameter

### Prosedur

Struktur Umum
```
procedure NamaProsedur(<input/output> param1: type1, <input/output> param2: type2, <input/output> parametc: typeetc)
{ Spek prosedur }
{ I.S. Initial State }
{ F.S. Final State }

KAMUS LOKAL
{ Nama variabel : type variabel }

ALGORITMA
{ Sederet instruksi, bebas mau apa aja }
```

Pemanggilan
```
NamaProsedur(param1, param2, parametc)
```

Catatan: 
* Jumlah parameter bebas, bisa juga tanpa parameter
* Setiap parameter bisa dijadikan input, output, atau keduanya (input/output)

## Loop

### Repeat N Times

Pengulangan berdasarkan banyak pengulangan
```
repeat n times
    { n bilangan bulat terdefinisi }
    <aksi>
```

### Repeat-Until

Pengulangan sampai kondisi berhenti, cek kondisi di akhir
```
repeat
    <aksi>
until <kondisi-berhenti>
```

### While

Pengulangan sampai kondisi berhenti, cek kondisi di awal
```
while <kondisi-loop> do
    <aksi>
```

### Iterate-Stop

Gabungan bentuk while dan repeat-until, cek kondisi di tengah (di bagian stop)
```
iterate
    <aksi-1>
stop <kondisi-berhenti>
    <aksi-2>
```

### For/Traversal

```
<pencacah> traversal [valMin..valMax]
    <instruksi>
```

Note: pencacah biasanya diisi nama i, j, k, atau lainnya.

Contoh:

```
i traversal [0..8]
    output(i)
```
