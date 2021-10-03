---
title: Berkenalan Dengan Bahasa Pemrogaman Javascript
created: 03-10-2021
update: -
---
# 1. Berkenalan dengan Javascript
javascript merupakan bahasa pemrogaman yang dibuat dengan tujuan pengembangan website agar lebih dinamis dan interaktif. Di pemrogaman web pada sebelumnya hanya menggunakan HTML CSS dan serverside menggunakan PHP kita dapat membuat sebuah website yang dinamis tetapi kurang interaktif terhadap usernya, tetapi dengan javascript kita dapat membuat semua hal yang tidak mungkin dilakukan sebelumnya jadi mungkin.

## Sejarah Javascript
Di tahun 1994 javascript mulai dikenal pada saat itu, di waktu itu juga web dan internet sudah mulai berkembang, Javascript sendiri dibuat oleh Brendan Eich yang merupakan karyawan Netscape. sebelum dinamai Javascript dulu juga sempat bergonta ganti nama dari Mocha, Mona, Livescript, dan pada akhirnya kita kenal saat ini namanya Javascript.

## Serverside menggunakan Javascript
javascript saat ini juga dapat digunakan sebagai bahasa pemrogaman untuk menangani process dalam server. NodeJS merupakan sebuah runtime javascript yang dirilis pada Mei 2009 dan dibuat oleh Ryan Lienhart Dahl dengan memisahkan Javascript Engine dari browser agar dapat digunakan diluar lingkungan browser atau dapat berjalan dilingkungan sistem operasi seperti MacOS, Windows, Linux dengan memanfaatkan google V8 Javascript Engine untuk menjalankan kode Javascript di lingkungan Sistem Operasi

## Seperti apa kode Javascript ?
- mengeluarkan output ke console
  ```javascript
    console.log("Hello World")
  ```
- deklarasi variabel
  ```javascript
  var nama = "Izzudin"
  let umur = 20
  const jeniskelamin = "laki-laki"
  ```
- Kondisi
  ```javascript
    if(jeniskelamin == "laki-laki"){
        console.log("saya adalah laki-laki yang kuat")
    }else{
        console.log("saya adalah perempuan yang cerdas")
    }
  ```
- Perulangan
  ```javascript
    for(let i = 1; i <= 5; i++){
        console.log("Perulangan ke-"+i)
    }
    
    let angka = 1
    while(angka < 10){
        console.log("angka kurang dari 10")
    }
  ```
- Fungsi
  ```javascript
    function cetakNama(nama){
        console.log("Namaku adalah" + nama)
    }
    
    //deklarasi fungsi seperti deklarasi variabel dengan arrow function
    const cetakUmur = (umur) => {
        console.log("umurku adalah" + umur)
    }
  ```

## Satu Bahasa untuk berbagai hal
Javascript disaat ini sendiri sudah berkembang lebih modern dalam menyelesaikan masalah, dulu Javascript hanya ditulis dengan istilah vanilla Javascript yang umumya digunakan di browser. Tetapi pada saat ini sudah berkembang seperti menjadi Runtime Nodejs yang dapat digunakan membangun berbagai aplikasi di sistem operasi manapun contohnya:
- Mobile
  platform android dan IOS merupakan platform yang umum digunakan untuk smartphone, kenapa mobile? karena dengan menggunakan aplikasi mobile kita dapat mengakses berbagai fitur lebih leluasa pada smartphone dari pada menggunakan web, Javascript sendiri memiliki Libary React Native untuk mengembangkan Aplikasi Mobile pada Smartphone yang menggunakan NodeJS sebagai runtime.
- Serverside
  seperti dijelaskan diatas Javascript sendiri dapat berjalan pada lingkungan sistem operasi sehingga kita dapat membangun aplikasi serverside menggunakan Javascript dan dijalankan oleh NodeJS, beberapa library Javascript berikut yang sering digunakan dalam pengembangan server:
  - ExpressJS untuk membangun web server
  - TypeORM dan Sequelize sebagai library ORM database
- Frontend
  memang sebelumnya tujuan Javascript adalah membuat User Interface pada web agar lebih interaktif, tetapi sekarang Javascript sudah berkembang lebih baik untuk user, dengan adanya javascript website saat ini dapat dikembangkan menjadi Single Page Application, Progressive Web Application dengan menggunakan beberapa Library seperti VueJS, ReactJS, Angular, Svelte.