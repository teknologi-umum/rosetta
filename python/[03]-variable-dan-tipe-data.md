---
title: Variable dan Tipe Data
created: 08-10-2021
update: -
---

# 3. Variable dan Tipe Data
---------------------------
Variable dan tipe data merupakan bagian yang tidak pernah terpisahkan dalam bahasa pemrograman. Pada bab ini akan dibahas mengenai dua hal tersebut.

## I. Basic Python
------------------
Sebelum masuk ke bagian yang lebih dalam, terdapat beberapa hal yang perlu menjadi perhatian dalam Python, antara lain sebagai berikut.

### A. Script Python
> Python merupakan suatu bahasa pemrograman yang memiliki extension .py. Sebuah script Python dapat ditulis pada Python interactive shell (CMD) maupun teks editor untuk dapat dijalankan.

### B. Indentasi Python
> Pada bahasa pemrograman lainnya, indentasi atau teks kosong sering dijadikan untuk menambah keterbacaan program. Namun, pada Python, indentasi ini digunakan sebagai aturan untuk memisahkan baris program.  

### C. Baris Komentar Python
> Baris komentar (Comment) merupakan baris yang tidak akan dijalankan oleh program. Seorang developer umumnya memanfaatkan baris ini untuk memberikan penjelasan terkait program yang dibuatnya. Pada Python terdapat dua jenis penerapan komentar.

#### i. Single Line Comment
> Janis komentar ini menggunakan tanda `#` untuk memberikan komentar perbaris

```python
    # Baris pertama komentar
    # Baris kedua komentar
```

#### ii. Multiline Comment
> Jenis komentar ini menggunakan tanda `"` sebanyak tiga kali untuk memberikan komentar beberapa baris sekaligus

```python
"""Semua tulisan ini tidak
akan dijalankan oleh Python
karena termasuk ke dalam 
komentar multiline
"""
```

## II. Tipe Data
----------------
Python memiliki beberapa tipe data. Tipe data yang paling sering kita gunakan nantinya sering 
disebut sebagai *primitive data*. Tipe data primitif ini terdiri dari string, number, dan boolean.

### A. Tipe Data String (Teks)
Tipe data string atau teks adalah tipe data yang digunakan untuk menyimpan suatu teks. Tipe data jenis ini diapit oleh tanda petik baik petik satu `('')` maupun petik dua `("")`. 

```python
'Namaku Anna'
"Ayahku seorang pebisnis"
```

Kedua contoh di atas memiliki tipe data string.

### B. Tipe Data Number (Angka)
Tipe data number atau angka adalah tipe data yang digunakan untuk menyimpan suatu angka. Tipe data number ini masih dipecah lagi menjadi tiga jenis yaitu **integer**, **float**, dan **kompleks**

#### i. Integer
Tipe data jenis ini merupakan tipe data yang merujuk angka dalam bilangan bulat.

```python
# Berikut contoh angka integer
10
100
1000
```

#### ii. Float
Tipe data jenis ini merupakan tipe data yang merujuk angka dalam pecahan/desimal.

```python
# Berikut contoh angka float
2.5
7.5
10.25
```

#### iii. Complex
Tipe data jenis ini merupakan tipe data yang merujuk pada nilai imajiner

```python
# Berikut contoh angka complex

15x + 10x = 25x
```

### C. Tipe Data Boolean
Tipe data ini adalah tipe data yang hanya terdiri dari dua buah nilai `True` dan `False`. Nilai `True` berarti benar dan `False` berarti salah. Meskipun hanya terdiri dari dua buah nilai tipe data ini sangat pentinga dalam membuat program dalam segala ukuran, baik kecil maupun besar.

```python
saya_manusia = True

print("Apakah anda seorang manusia?", saya_manusia)
```
Tipe data boolean sering dikaitkan dengan `operator logika` yang mana pembahasan terhadap hal tersebut tidak dibahas pada materi ini. Tetapi sebagai referensi dapat mengakses halaman [wikipedia](https://id.wikipedia.org/wiki/Operator_logika). Dari operator logika inilah terbentuklah program yang kompleks seperti menggunakan if else.

```python
umur = 18

if umur >= 17:
	print("Bisa memperoleh SIM")
else:
	print("Belum dapat memperoleh SIM")
```

## III. Variable
--------------
Setelah memahami konsep tipe data, kita akan membahas suatu variable. Untuk memudahkan dalam memahami hal ini, anggaplah tipe data sebagai suatu kelereng dan variable sebagai suatu toples. Tentu untuk merapikan kelereng yang tercecer kita akan memasukkannya ke dalam toples bukan?. Nah dalam pemrograman juga sama, untuk membuat program yang besar dan berkelanjutan diperlukan banyak toples (variable) untuk menyimpan data yang tercecer.

### A. Bagaimana Membuat Suatu Variable?
Python sangat memudahkan penggunanya dalam menuliskan variable. Cukup dengan menuliskan penamaan untuk variable lalu diikuti nilai yang hendak disimpan, contoh sebagai berikut.

```python
nama = 'Handhika Yanuar Pratama'
usia = 24.5
punya_pacar = False
```
Pada contoh di atas kita telah menyimpan beberapa data ke dalam tiga buah variable, untuk memanggilnya, cukup menyisipkannya dalam script yang hendak dibuat.

```python
print("Nama saya:", nama)
print("Umur saya:", usia)
print("Saya sudah punya pacar:", punya_pacar)
```
Nah ketika dijalankan maka variable akan dipanggil ke dalam program

```shell
Nama saya: Handhika Yanuar Pratama
Umur saya: 24.5
Saya sudah punya pacar: False
```

### B. Bagaimana Aturan Menulis Variable?
Python memiliki aturan dalam memberikan penulisan variable, antara lain:
1. Nama variable hanya dapat diawali oleh huruf atau underscore (contoh: nama, _nama)
2. Nama variable tidak dapat diawali dengan angka (contoh: ~8nama~)
3. Nama variable hanya terdiri dari karakter alpha-numeric dan underscore saja (a-z, A-Z, 0-9, & _)
4. Nama variable bersifat case sensitive, jadi ketika terdapat perbedaan penulisan seperti `Love` dan `love` kedua nilai tersebut merepresentasikan nilai yang berbeda.

### C. Bagaimana Menyimpan Data Pada Variable?
Untuk menyimpan data pada suatu variable terdapat dua buah cara baik secara single maupun multiple. Penyimpanan secara single artinya menyimpan suatu data pada sebuah variable saja. Sedangkan penyimpanan secara multiple artinya menyimpan beberapa data sekaligus ke dalam variable. 

```python
# Contoh penyimpanan single
a = 10
nama = 'Vega'

# Contoh penyimpanan multiple
x, y, z = 10, 2.5, 'Lin'
```

Selain dua hal tersebut, pada Python juga mendukung penyimpanan suatu nilai yang sama untuk beberapa variable dengan syntax sebagai berikut

```python
a = b = c = d = 20
```

### D. Bagaimana Mengetahui Tipe Data Suatu Variable?
Setelah paham konsep tipe data dan variable. Tentu pertanyaan ini sering muncul, pada bahasa Python, jawaban dari pertanyaan ini cukup sederhana yaitu menggunakan perintah `type(nama_variable)`. 

```python
buah = 'apple'
jumlah = 5

type(buah)
type(jumlah)
```

Maka output dari perintah tersebut yaitu
```python
<type 'str'>
<type 'int'>
```

---
Cukup mudah bukan, bahasan terkait variable dan tipe data ini. Sebenarnya masih terdapat beberapa tipe data lainnya, seperti list, tuple, dan dictionaries yang akan dibahas lebih lanjut pada bagian berikutnya.
