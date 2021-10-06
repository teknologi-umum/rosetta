---
title:  Pengantar Haskell 
created: 04-10-2021
update: -
---

# 1. Pengantar Haskell

Haskell adalah bahasa pemrograman fungsional dan serba guna. Haskell muncul pada tahun 1990, 
standar bahasa Haskell tercatat dari 4 Oktober 2021 yaitu Haskell 2010 dengan versi implementasi :
GHC (9.0.1).

## 1.1 Fitur

Setiap bahasa memiliki kelebihanya tersendiri, bukan? maka berikut ini fitur yang Haskell tawarkan kepada kamu.

### Tipe Statis

Haskell menindak bagian program sebagai ekspresi dan setiap ekspresi memiliki tipe yang menentukan jenis data apa yang bisa diterima. Tipe statis menahan perubahan tipe data dari suatu ekpresi untuk menjaga kekonsistenan bentuk ekspresi.

Rupa tipe statis pada Haskell dan Javascript :

- Haskell

    ```haskell
    nama :: String 
    nama = "Elsavina"

    nama = 123 -- akan error
    ```

- Javascript

    ```javascript
    nama = "Elsavina"

    nama = 123
    // works fine
    ```

### Inferensi Tipe

Inferensi tipe memperbolehkan suatu ekspresi menentukan tipe dari operator dan nilai yang diterima, ini menghemat kita untuk tidak berulang kali menuliskan tipe pada ekspresi.

```haskell
namaLengkap = "Rismawati Nurfitri"
-- namaLengkap akan bertipe string
-- gunakan :t namaLengkap pada GHCI
-- untuk membuktikan ini
```

### Paradigma Fungsional

Paradigma fungsional merupakan kerangka pikir untuk menalar permasalahan dengan pendekatan fungsi matematis. Ada empat prinsip utama yang perlu diperhatikan untuk menentukan suatu bahasa termasuk paradigma fungsional yaitu

- Fungsi Orde Tinggi (_High-order Function_)
- _Referential Transparency_ (Nilai dari sebuah variable tidak berubah)
- Fungsi Murni (_Pure Function_)
- Rekursi

Mata kunci untuk memahami paradigma fungsional yaitu paradigma ini lebih menekankan pembangkitan nilai baru daripada merubah nilai lama untuk menghasilkan nilai yang kita inginkan.

Haskell memiliki dukungan penuh terhadap paradigma ini.

### Evaluasi Malas 

Haskell tidak akan menjalankan sebuah ekspresi yang tidak mengeluarkan efek samping seperti menampilkan sesuatu atau berurusan dengan Input/Output, pendekatan ini memberikan penghematan performa yang bagus karena tidak men-compile bagian yang tidak memiliki efek namun sulit untuk memprediksi benchmark dari sebuah program.

## 1.2 Kasus Guna 

Haskell bukan bahasa populer namun bukan berarti tidak memiliki implementasi pada kasus tertentu. Haskell banyak digunakan untuk menuliskan rumus ilmiah, membangun kompilator dan berurursan dengan aplikasi bisnis tertentu (seperti Web API server dan semacamnya).

- [Elm](https://elm-lang.org) merupakan salah satu bahasa pemrograman yang kompilatornya dibangun menggunakan Haskell.

- [NoRedInk](https://news.ycombinator.com/item?id=17600231) merupakan salah satu perusahan digital yang bergerak dalam bidang pendidikan untuk menyediakan pelajaran menulis dan telah melayani pembelajaran 50% sekolah menengah atas di Amerika.

## 1.3 Referensi Belajar

Kamu tertarik untuk belajar Haskell maka kamu datang dijalan yang benar. Selain repositori ini, kamu bisa mempelajari haskell melalui referensi berikut:

- [Awesome-like untuk Pemrograman Fungsional](https://github.com/artileda/pemrograman-fungsional)
- [1. Pengantar Haskell | Seri Haskell - Idiosemantik](https://www.youtube.com/watch?v=BSWoegYLC3E)