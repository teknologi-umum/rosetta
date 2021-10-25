---
title: Variabel dan Operator Pada Javascript
created: 20-10-2021
update: 22-10-2021
---

# Apa itu variabel
Variabel sendiri merupakan tempat yang digunakan untuk menyimpan sebuah state atau data, data yang disimpan bisa berupa tipe data string, boolean, integer, dsb. Javascript sendiri merupakan bahasa pemrograman berjenis `typeless` yang artinya satu variabel dapat berisi tipe data apapun.

## Deklarasi Variabel
Deklarasi variabel di Javascript memiliki berbagai cara seperti : 
### var
```javascript
var nama = "Ahmad"
var umur = 12
```
var merupakan sebuah kalimat yang kita gunakan untuk mendeklarasikan sebuah variabel global, sebelum adanya fitur ES6 pada javascript deklarasi var sendiri memiliki banyak masalah seperti :
- Variabel global
  Variabel global memiliki cenderung memiliki masalah saat deklarasi maupun tidak dideklarasikan seperti :
  ```javascript
  mahasiswa = "akbar" // output -> akbar
  //variabel yang tidak diklarasikan
  ```
  Contoh tersebut tidak menimbulkan error karena javascript menganggap mahasiswa merupakan variabel global sehingga jika program javascript kompleks dapat membuat kita bingung.
- Deklarasi ganda
  Ada lagi hal aneh saat kita menggunakan var yaitu deklarasi variabel ganda dengan nama yang sama seperti contoh berikut :
  ```javascript
    var nama = "ahmad"
    var nama = "rafi"
    console.log(nama) // output -> rafi
  ```
  Potongan kode diatas akan menghasilkan output "rafi". Meskipun deklarasi awal variable nama diberikan nilai "ahmad". Akan tetapi kita dapat mendeklarasikan ulang variable dengan identifier yang sama yakni nama dan memberikan value yang berbeda dalam hal ini disebut sebagai reassign atau diganti isinya.
- Hoisting
  Jika kita mendeklarasikan sebuah variable pada javascript maka yang terjadi adalah javascript mengangkat semua variable keatas kemudian mengeksekusinya. Meskipun anda menempatkan variable diakhir baris kode maka javascript akan tetap mengangkat variable keatas sebelum mengeksekusinya.
  ```javascript
    hallo = "hello world" // mengisi variable hallo 
    console.log(hallo) // menampilkan variable hallo
    var hallo // variable hallo akan diangkat keatas sebelum dieksekusi
  ```

### let
```javascript
let nama = "ahmad"
let umur = 15
```
Deklarasi variabel let berfungsi sama halnya dengan var tetapi menggunakan let kita dapat mengatasi berbagai masalah yang ada saat menggunakan var, tidak hanya itu scope juga merupakan hal yang penting saat menggunakan let contohnya
```javascript
let gender = "male"

function getNama(){
    let nama = "ahmad"
    console.log(nama)
}
function getUmur(){
    let umur = 12
    console.log(12)
}

console.log(gender) // output -> male
console.log(nama) // error
console.log(umur) // error
getNama() // output -> nama
```
Saat kita ingin memanggil variabel umur dan nama didalam scope fungsi akan terjadi error karena ruang lingkup variabelnya berbeda, tetapi saat memanggil fungsi tersebut tidak terjadi error karena ruang lingkup variabel tersebut ada di fungsi yang kita panggil.


### const
```javascript
const nama = "Rafi"
const gender = "male"
```
const merupakan bentuk deklarasi variabel immutable yang artinya variabel yang kita deklarasikan tidak dapat berubah-ubah isinya, contohnya :
```javascript
let umur = 12 // deklarasi umur
umur = 13 // reassign atau mengganti nilai umur
const nama = "ahmad" //deklarasi ahmad
nama = "rafi" //error
```
Dapat dilihat pada potongan kode tersebut saat kita mengganti variabel umur setelah deklarasi maka nilai tersebut berubah hal ini dikarenakan karena kita menggunakan let yang artinya deklarasi tersebut bersifat mutable yang mana nilainya dapat berubah-ubah, berbeda halnya dengan menggunakan const kita tidak bisa merubah nilainya.


# Operator
Operator merupakan simbol yang digunakan untuk melakukan operasi tertentu pada suatu nilai dan variabel.
Operator Bahasa Pemrogaman sendiri terbagi dalam 4 jenis :
- Operator Aritmatika
- Operator Penugasan
- Operator Perbandingan
- Operator Logika

## Operator Aritmatika pada Javascript
Operator aritmatika merupakan operator yang digunakan untuk melakukan fungsi penjumlahan, pengurangan, pembagian, perkalian, dsb.
Operator aritmatika terdiri dari : 
| Nama Operator | Simbol |
| ------------- | -- |
| Penjumlahan   | + |
| Pengurangan   | - |
| Perkalian     | * |
| Pemangkatan   | ** |
| Pembagian     | / |
| Modulus       | % |

Contoh penggunakan operator Aritmatika : 
```javascript
let a = 10
let b = 5

console.log(a + b) // 15
console.log(a - b) // 5
console.log(a * b) // 50
```

Operator aritmatika juga dapat digunakan sebagai penggabungan teks seperti :
```javascript
let namaDepan = "Rafi"
let namaBelakang = "Ahmad"
let fullName = namaDepan + " " + namaBelakang
console.log(fullName) // Rafi Ahmad
```

## Operator Penugasan pada Javascript
Operator Penugasan adalah operator yang digunakan untuk memberikan tugas kepada variabel. Biasanya digunakan untuk mengisi variabel.
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
Operator Perbandingan adalah operator yang digunakan untuk membandingkan dua nilai.

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
Perlu diketahui saat kita menggunakan 2 tanda sama dengan dengan 3 tanda sama dengan maka statementnya dapat berubah, contohnya : 
```javascript
console.log(1 == "1") // true
console.log(1 === "1") //false
```
Mengapa hal tersebut dapat terjadi saat kita menggunakan operator perbandingan? Karena di Javascript saat kita menggunakan 2 tanda sama dengan, kita melakukan komparasi nilainya tanpa mengenal tipe datanya, berbeda saat kita menggunakan 3 tanda sama dengan, kita melakukan komparasi nilainya beserta tipe datanya.
Tidak hanya operator perbandingan equal, menggunakan operator NOT `!` juga hal serupa
```javascript
console.log(1 != "1") //false
console.log(1 !== "1") // true
```
Dapat dilihat dari potongan kode tersebut bahwa statement pertama menunjukan NOT 1 tidak sama dengan "1"  dapat mengeluarkan output false dikarenakan 1 harusnya sama dengan "1" karena nilainya sama tetapi karena kita menggunakan operator NOT `!` hal tersebut berubah terbalik. Sama halnya dengan 1 !== "1" yang berarti false karena nilainya sama tetapi tipe datanya tidak sama harusnya mengeluarkan output false, tetapi dengan menggunakan operator NOT `!` hal tersebut berubah menjadi terbalik. 

# Operator Logika pada javascript
Operator logika digunakan untuk melakukan operasi terhadap dua nilai boolean.

Operator ini terdiri dari :
| Nama Operator | Simbol |
| ------------- | ------ |
| Logika AND    | `&&`     |
| Logika OR     | `||`      |
| Negasi        | `!`      |

contoh : 
```javascript
let benar = true
let salah = false

console.log(benar || salah) // true
console.log(benar && salah) // salah
console.log(!benar && salah) // true
```

