---
title: Variabel dan Operator
created: 25-10-2023
update: -
---

## Variabel Dalam Golang
Variabel digunakan untuk menyimpan data dalam Go. Go memiliki aturan ketat tentang deklarasi dan penggunaan variabel. Berikut adalah cara mendeklarasikan variabel dalam Go:

```go 
var namaVariabel tipeData
```

Contoh penggunaan variabel: 
```go
var umur int
umur = 25
```

Variabel juga dapat dideklarasikan dengan inisialisasi sekaligus:

```go
var nama string = "John"
```

Go juga mendukung deklarasi pendek menggunakan `:=`

```go
umur := 14
nama := "Refaldy"
```
## Tipe Data Di Go
#### 1. Tipe Data Angka (Numerik)
<li>int: Digunakan untuk menyimpan nilai bilangan bulat, misalnya int dan int64.</li>
<li>uint: Digunakan untuk bilangan bulat tanpa tanda (non-negatif), misalnya uint dan uint32.</li>
<li>float32 dan float64: Digunakan untuk bilangan pecahan (floating-point numbers).</li>

Contoh: 
```go
var umur int
var beratBadan float64
```

#### 2. Tipe Data String
<li>string: Digunakan untuk menyimpan teks atau karakter.</li>
Contoh:

```go
nama := "Alice"
var email string
```

#### 3. Tipe Data Boolean
<li>bool: Hanya memiliki dua nilai mungkin, yaitu true dan false.</li>
Contoh

```go
aktif := true
var isAdmin bool
isAdmin = false
```

#### 4. Tipe Data Karakter (Character Type)
<li>byte: Digunakan untuk menyimpan data biner atau karakter tunggal.</li>
<li>rune: Digunakan untuk menyimpan karakter Unicode.</li>

Contoh:
```go
var karakter byte
var simbol rune
```

#### 5. Tipe Data Array
<li>array: Digunakan untuk menyimpan kumpulan elemen dengan tipe data yang sama dan ukuran tetap.</li>

Contoh:
```go
var angka [5]int
```

#### 6. Tipe Data Slice
<li>slice: Digunakan untuk menyimpan potongan dari array atau slice lain. Tidak memiliki ukuran tetap.
</li>

Contoh: 
```go
data := []int{1, 2, 3, 4, 5}
```
atau
```go
var data [3]int
data = [3]int{1, 2, 3}
sliceData := data[1:2] //[2]
```

#### 7. Tipe Data Map
<li>map: Digunakan untuk menyimpan pasangan key-value, mirip dengan kamus.</li>

Contoh:
```go
nilai := map[string]int{"Matematika": 90, "Bahasa": 85}
```

#### 8. Tipe Data Struct
<li>struct: Digunakan untuk mendefinisikan tipe data yang dapat memiliki beberapa bidang (fields) dengan tipe data yang berbeda.</li>

Contoh: 
```go
type Mahasiswa struct {
    Nama string
    Umur int
}
```

#### 9. Tipe Data Interface
<li>interface: Digunakan untuk mendefinisikan kontrak antara tipe data, memungkinkan polimorfisme.</li>

Contoh:
```go
type Bentuk interface {
    Luas() float64
}
```

#### 10. Tipe Data Pointer
<li>pointer: Digunakan untuk menyimpan alamat memori variabel lain.</li>
Contoh:

```go
var x int
var ptr *int
ptr = &x
```

## Zero Values
Setiap variabel di Go memiliki nilai awal atau "zero value" yang terkait dengan tipe datanya. Contoh "zero values" yang umum:

<li><b>int</b> memiliki zero value 0.</li>
<li><b>float64</b> memiliki zero value 0.0.</li>
<li><b>bool</b> memiliki zero value false.</li>
<li><b>string</b> memiliki zero value "" (string kosong).</li>

## Operator Di Go
Go mendukung berbagai operator aritmatika, perbandingan, logika, dan lainnya. Beberapa contoh operator yang umum digunakan:

### Operator Aritmatika
```go
a := 10
b := 5
penjumlahan := a + b
pengurangan := a - b
perkalian := a * b
pembagian := a / b
sisa := a % b
```
### Operator Perbandingan
```go
a := 10
b := 5
samaDengan := a == b
tidakSama := a != b
lebihBesar := a > b
kurangDari := a < b
lebihBesarSamaDengan := a >= b
kurangDariSamaDengan := a <= b
```
### Operator Logika
```go
benar := true
salah := false
logikaAnd := benar && salah
logikaOr := benar || salah
logikaNot := !salah
```

## Pointer Di Golang
Pointer adalah variabel yang menyimpan alamat memori dari variabel lain. Mereka digunakan untuk mengakses dan memanipulasi variabel asli. Contoh penggunaan pointer:

```go
a := 15
var pointerA *int
pointerA = &a
*pointerA = 20 // Mengubah nilai a menjadi 20
```

## Iota Itu Apa?
iota adalah konstanta yang digunakan dalam konstanta enumerasi. Ini secara otomatis diinkrementasi pada setiap konstanta berikutnya dalam blok konstanta.

```go
const (
    Senin = iota
    Selasa
    Rabu
    Kamis
    Jumat
    Sabtu
    Minggu
)
```
Dalam contoh di atas, iota dimulai dari 0 dan diinkrementasi setiap kali ada konstanta baru.