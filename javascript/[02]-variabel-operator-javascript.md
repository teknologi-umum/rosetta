---
title: Variabel dan Operator Pada Javascript
created: 20-10-2021
update: -
---

# Apa itu variabel
variabel sendiri merupakan tempat yang digunakan untuk menyimpan sebuah state atau data, data yang disimpan bisa berupa tipe data string, boolean, integer, dsb. Javascript sendiri merupakan bahasa pemrograman berjenis `typeless` yang artinya satu variabel dapat berisi tipe data apapun.

## Deklarasi Variabel
deklarasi variabel di Javascript memiliki berbagai cara seperti : 
### var
var merupakan sebuah kalimat yang kita gunakan untuk mendeklarasikan sebuah variabel global, cara ini tidak direkomendasikan untuk mendeklarasikan variabel karena scope dalam var adalah global, berikut adalah cara deklarasi variabel global dan penggunaannya
```javascript
var nama = "Ahmad"
var umur = 12
```

### let
deklarasi variabel let berfungsi sama halnya dengan har tetapi menggunakan let kita tidak bisa mengakses variabel secara sesuka hati dikarenakan let berada dalam scope tertentu
```javascript
let nama = "ahmad"
let umur = 15

nama = "Rafi"
console.log(nama) //Rafi
function setGender(){
    let gender = "Male"
}
console.log(gender) // Error
```

### const
const merupakan bentuk deklarasi variabel immutable yang artinya variabel yang kita deklarasikan tidak dapat berubah-ubah isinya
```javascript
const nama = "Rafi"
let umur = 12

umur = 13 // Umur menjadi 13
nama = "Ahmad" // Error
```

# Operator
operator merupakan simbol yang digunakan untuk melakukan operasi tertentu pada suatu nilai dan variabel.
Operator Bahasa Pemrogaman sendiri terbagi dalam 6 jenis :
- Operator Aritmatika
- Operator Penugasan
- Operator Perbandingan
- Operator Logika

## Operator Aritmatika pada Javascript
operator aritmatika merupakan operator yang digunakan untuk melakukan fungsi penjumlahan, pengurangan, pembagian, perkalian, dsb.
operator aritmatika terdiri dari : 
| Nama Operator | Simbol |
| ------------- | -- |
| Penjumlahan   | + |
| Pengurangan   | - |
| Perkalian     | * |
| Pemangkatan   | ** |
| Pembagian     | / |
| Modulus       | % |

contoh penggunakan operator Aritmatika : 
```javascript
let a = 10
let b = 5

console.log(a+b) // 15
console.log(a-b) // 5
console.log(a*b) // 50
```

operator aritmatika juga dapat digunakan sebagai penggabungan teks seperti :
```javascript
let namaDepan = "Rafi"
let namaBelakang = "Ahmad"
let fullName = namaDepan + " " + namaBelakang
console.log(fullName) // Rafi Ahmad
```

## Operator Penugasan pada Javascript
Operator penugasan adalah operator yang digunakan untuk memberikan tugas kepada variabel. Biasanya digunakan untuk mengisi variabel.
Operator penugasan terdiri dari : 
| Nama Operator | Simbol |
| ------------- | ------ |
| Pengisian Nilai | = |
| Pengisian dan penambahan | += |
| Pengisian dan pengurangan | -= |
| Pengisisan dan perkalian | *= |
| Pengisian dan pemangkatan | **= |
| Pengisian dan pembagian | /= |
| Pengisian dan modulus | %= |

contoh : 
```javascript
let pengunjung = 10

//contoh penulisan tanpa operator penugasan
pengunjung = pengunjung + 1

//contoh penulisan dengan operator penugasan
pengunjung += 1
```

## Operator Perbandingan pada Javascript
Operator perbandingan adalah operator yang digunakan untuk membandingkan dua nilai.

Operator perbandingan akan menghasilkan sebuah nilai boolean true dan false.

Operator perbandingan terdiri dari :
| Nama Operator | Simbol |
| ------------- | ------ |
| Lebih Besar   | > |
| Lebih Kecil   | < |
| Sama Dengan   | == atau === |
| Tidak Sama dengan | != atau !== |
| Lebih Besar sama dengan | >= |
| Lebih Kecil sama dengan | <= |

contoh :
```javascript
let a = 10
let b = 5

console.log(a > b) // true
console.log(a < b) // false
console.log(a == b) // false
console.log(a != b) // true
```

# Operator Logika pada javascript
Operator logika digunakan untuk melakukan operasi terhadap dua nilai boolean.

Operator ini terdiri dari :
| Nama Operator | Simbol |
| ------------- | ------ |
| Logika AND    | &&     |
| Logika OR     | ||     |
| Negasi        | !      |

contoh : 
```javascript
let benar = true
let salah = false

console.log(benar || salah) // true
console.log(benar && salah) // salah
console.log(!benar && salah) // true
```

