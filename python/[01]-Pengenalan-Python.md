---
title: Berkenalan Dengan Bahasa Pemrogaman Python
created: 04-10-2021
update: -
---

# 1. Berkenalan dengan Python

Python merupakan bahasa pemrograman yang sangat populer dan tumbuh dengan sangat cepat. Bahasa ini sangat mudah dipahami bahkan untuk pemula. Syntax yang sederhana menjadikannya sangat direkomendasikan untuk dipelajari pertama kali dalam bahasa pemrograman. Dibandingkan yang lain, bahasa ini memiliki cakupan sangat luas mulai dari pemrograman dasar, aplikasi desktop, aplikasi web, aplikasi mobile, hingga Machine learning dapat dikerjakan menggunakan bahasa ini.

## Sejarah Python

Python didesainn oleh Guido Van Rossum dari Centrum Wiskunde & Informatica(CWI) dan dikembangkan
oleh Python Software Foundation. Terdapat banyak sumber yang menyatakan Python resmi dibuat tahun
1989, 1990, ataupun 1991. Perbedaan tersebut bukanlah hal yang seharusnya diperdebatkan. Hal ini
dikarenakan, tujuan utama dibuat Python yaitu untuk source code program yang mudah dibaca dan syntax yang membuat seorang programmer dapat mengekspresikan hal yang diinginkannya dengan baris kode yang sedikit.

## Python sebagai interpreted language

Bahasa python merupakan sebuah bahasa interpreted artinya sebelum dijalankan program akan memeriksa keseluruhan syntax, kemudian memeriksanya lalu melakukan compiling dan merubahnya menjadi bytecode. Bytecode pada python ini berekstensi .pyc yang mana proses ini berjalan secara internal oleh sistem dan tersembunyi dari developer. Selanjutnya dari bytecode dinterpertasikan ke memory untuk dijalankan. Intinya, ketika kita menjalankan program Python kita tidak perlu repot-repot memikirkan compiling seperti keluarga bahasa C karena semua sistem akan bekerja dibalik layar developer.

## Python 2 dan Python 3

Terdapat dua jenis bahasa Python yang berkembang hingga tahun 2020 yaitu Python 2 dan Python 3. Perkembangan Python 2 dimulai sejak tahun 2000, versi terakhirnya yaitu versi 2.7 yang pada tahun 2020 sudah tidak dilanjutkan lagi pengembangannya. Python 3 pertama kali dirilis Desember 2008, versi ini merupakan perbaikan untuk Python 2. Terdapat banyak perubahan dari Python 2 ke Python 3 sehingga pada bahasan ini akan berfokus pada bahasa Python 3.

## Seperti apa kode Python ?

- Mengeluarkan output
  ```python
    print("Hello World")
  ```
- Deklarasi variabel
  ```python
  nama = "Handhika"
  umur = 20
  jenis_kelamin = "pria"
  ```
- Kondisi
  ```python
    if jenis_kelamin == "pria":
        print("saya adalah seorang pria")
    else:
        print("saya adalah seorang perempuan")
  ```
- Perulangan

  ```python
    for i in range(10):
        print("Perulangan ke-{}".format(i))

    nomor = 1
    while (nomor < 10):
        print("Sekarang nomor antrian:", nomor)
  ```

- Fungsi

  ```python
    def namamu(nama):
  	print("Namamu adalah:", nama)

  namamu("Ben")
  ```

## Python Sebagai Multi-Purpose Language

Penggunaan Python mencakup berbagai bidang dalam kehidupan sehari-hari, diantaranya:

1. Data Analysis
   Python hadir dengan banyak library yang memudahkan data science untuk bekerja. Seperti NumPy dan Pandas yang digunakan untuk pengolahan data maupun Matplotlib dan Seaborn yang digunakan untuk visualisasi data. Kelebihan ini menjadikan bahasa Python sangat direkomendasikan oleh banyak data scientists.

2. Automation dan Bots
   Keperluan akan otomatisasi kian hari kian mengalami peningkatan, Python merupakan bahasa yang sangat fleksibel sehingga tugas yang bersifat berulang-ulang seringkali dibuatkan otomatisasi oleh seorang administrator. Selain untuk otomatisasi, banyak bot yang dibangun menggunakan bahasa Python karena mudah dalam pembuatannya.

3. Web Application
   Python dapat digunakan untuk membuat suatu website. Dukungan library seperti Pyramid, Django, Flask, dan Streamlit menjadikan pemrograman ini menjadi salah satu pemrogaman web yang seringkali bersaing dengan JavaScript.

4. Desktop Application
   Python seringkali disejajarkan dengan keluarga bahasa C dalam membuat suatu desktop application. Library seperti tkinter, kivy, dan pyqt merupakan beberapa library yang sering digunakan untuk membuat aplikasi desktop (GUI)

5. Mobile Application
   Python mendukung pembuatan aplikasi untuk perangkat mobile maupun untuk membuat sebuah game. Beberapa library yang digunakan untuk membuatnya yaitu Kivy, Pygam, dan PyQt.

6. Data Crawling dan Web Scrapping
   Pengumpulan data merupakan tantangan terbesar bagi seorang data scientists dalam menjalankan tugasnya. Bahasa Python memiliki library yang dapat digunakan untuk melakukan parsing ke suatu situs dan melakukan pengambilan data dari situs tersebut untuk diolah. Library yang sering digunakan yaitu scrapy dan selenium

7. Network dan Security
   Python memudahkan banyak seorang administrator jaringan dalam menjalankan tugasnya, baik berupa pembuatan otomatisasi maupun juga untuk membuat pengaturan jaringan lainnya dengan hanya beberapa baris kode saja. Beberapa library seperti ftplib, requests dan subprocess juga disediakan Python dan mudah diimplementasikan. Selain itu, banyak tools hacking yang tersedia dibangun menggunakan bahasa Python sehingga Python sangat cocok dalam bidang ini.

8. Artificial Intelligence(AI), Machine Learning(ML) dan Deep Learning(DL)
   AI, ML, dan DL merupakan sebuah fields yang mendekatkan manusia dengan dunia robotic. Pemrograman Python sangat memungkinkan menyelesaikan permasalahan berkaitan hal ini. Dukungan library seperti tensorflow, scipy, dan scikit-learn seringkali menjadikan bahasa ini sangat direkomendasikan dibandingkan bahasa lain yaitu matplotlib dan R.

Delapan kelebihan diatas hanyalah beberapa manfaat dari bahasa Python, masih banyak yang dapat digali lebih jauh dari bahasa ini.
