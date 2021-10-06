---
title: Berkenalan Dengan Bahasa Pemrograman C
created: 06-10-2021
update: -
---
# 1. Berkenalan dengan C
Bahasa pemrograman C adalah sebuah bahasa pemrograman komputer yang bisa digunakan untuk membuat berbagai aplikasi (general-purpose programming language), 
mulai dari sistem operasi (seperti Windows atau Linux), antivirus, software pengolah gambar (image processing), hingga compiler untuk bahasa pemrograman, 
dimana C banyak digunakan untuk membuat bahasa pemrograman lain yang salah satunya adalah PHP.

## Sejarah C
Bahasa pemrograman C dibuat pertama kali oleh Dennis M. Ritchie pada tahun 1972. Saat itu Ritchie bekerja di Bell Labs, sebuah pusat penelitian yang berlokasi di Murray Hill, 
New Jersey, Amerika Serikat. Ritchie membuat bahasa pemrograman C untuk mengembangkan sistem operasi UNIX. Sebelumnya, sistem operasi UNIX dibuat menggunakan 
bahasa assembly. Akan tetapi bahasa assembly sendiri sangat rumit dan susah untuk dikembangkan.

Dengan tujuan mengganti bahasa assembly, peneliti di Bell Labs membuat bahasa pemrograman B. Namun bahasa pemrograman B juga memiliki beberapa kekurangan, 
yang akhirnya di lengkapi oleh bahasa pemrograman C. Dengan bahasa C inilah sistem operasi UNIX ditulis ulang. Pada gilirannya, UNIX menjadi dasar dari banyak 
sistem operasi modern saat ini, termasuk Linux, Mac OS, iOS, hingga sistem operasi Android.

## God’s programming language
Bahasa C juga dijuluki sebagai “God’s programming language” karena banyak menginspirasi bahasa-bahasa pemrograman yang lain seperti Java, Javascript, C++, C#, PHP, dsb.
Bahasa C memang bagus untuk memperkenalkan konsep pemrograman bagi pemula yang belum pernah coding, Usia bahasa pemrograman C memang cukup tua, 
namun masih digunakan hingga saat ini.



## Seperti apa kode C ?
- Mengeluarkan Output
  ```C
  #include <stdio.h>
  int main(void) {
      printf("Hello, World!\n");
      return 0;
  }
  ```
- Deklarasi Variabel
  ```C
  char name[] = "bryan"; //tipe data yang karakter
  int umur = 20;         //tipe data yang berupa angka
  float berat = 46.7;    //tipe data yang berupa bilangan pecahan
  double tinggi = 170.43;//sama seperti float, namun double memiliki ukuran penyimpanan yang lebih besar

  ```
- Kondisi
  ```C
  if (nilai == 'A' ) {
    printf("Pertahankan! \n");
  }
  else if (nilai == 'B' ) {
    printf("Harus lebih baik lagi \n");
  }
  else if (nilai == 'C' ) {
    printf("Perbanyak belajar \n");
  }
  else if (nilai == 'D' ) {
    printf("Jangan keseringan main \n");
  }
  else if (nilai == 'E' ) {
    printf("Kebanyakan bolos... \n");
  }
  else {
    printf("Maaf, format nilai tidak sesuai \n");
  }
  ```
- Perulangan IF ELSE
  ```C
  for (int i = 0; i < 10; i++) {
       printf("Perulangan ke-%i\n", i);
  }
  ```
- Perulangan WHILE
  ```C
  int i = 1;
  while (i <= 5){
    printf("Hello World \n");
    i++;
  }
  ```
- Perulangan DO WHILE
  ```C
  int i = 1;
  do {
    printf("Hello World \n");
    i++;
  }
  while (i <= 5);
  ```
- Fungsi
  ```C
  void say_hello() {
      printf("Hello Selamat Datang!\n");
  }

  void main(){
      // memanggil fungsi say_hello()
      say_hello();
  }
  ```

## Paradigma C

Bahasa C menggunakan paradigma procedural programming, dimana untuk menulis program yang kompleks, kode akan dipecah menjadi fungsi-fungsi yang saling terpisah untuk kemudian disatukan di dalam kode program utama. Keunggulan dari procedural programming adalah mudah dipelajari. Namun ketika masuk ke aplikasi yang kompleks, pengelolaan kode program akan menjadi kendala utama.
Misalnya jika kita mendefinisikan variabel bernama luas_lingkaran di satu tempat, maka variabel yang sama tidak bisa di tulis di tempat lain.

## Bahasa C Untuk Pemula
Seperti yang disebutkan sebelumnya, beberapa basis dari bahasa pemrograman ini digunakan pada beberapa jenis bahasa pemrograman yang baru.
Dengan kata lain, saat kita mempelajari bahasa pemrograman C dan menguasainya, secara tidak langsung kita juga mempelajari dasar-dasar dari bahasa pemrograman lainnya. 
Secara mendasar, dengan mengetahui bahasa pemrograman C, kita akan mendapatkan sebuah tiket untuk mengetahui hampir seluruh bahasa pemrograman.

Terdapat beberapa kegunaan dari bahasa ini. Termasuk di dalamnya, bahasa ini awalnya dibangun agar dapat digunakan untuk mengembangkan sistem perangkat lunak. 
Idealnya, bahasa pemrograman C dapat digunakan untuk membangun firmware maupun aplikasi portabel. Selain itu, bahasa pemrograman C dapat digunakan untuk 
mengembangkan sistem operasi ataupun sistem yang berhubungan dengan perangkat keras.

Kelebihan bahasa pemrograman C ini juga yang menyebabkan bahasa tersebut menjadi sangat populer di kalangan perusahaan teknologi, termasuk di dalamnya Intel, Amazon, 
dan DELL. Kepopuleran ini juga dapat menjadi salah satu kriteria yang digunakan dalam memilih bahasa yang tepat bagi yang ingin mulai belajar.
