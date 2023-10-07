---
title: Berkenalan Dengan Bahsa Pemrograman Assembly
created: 07-10-223
update: -
---

# 1. Berkenalan dengan Assembly
Assembly merupakan bahasa pemrograman tingkat rendah yang berarti berhubungan dengan kerangka komputer atau bagaimana CPU bekerja.
Tentunya kode assembly tidak portable dikarenakan perbedaan jenis CPU, Sistem Opera64si, serta ABI.
Bahasa digunakan saat menganalisis malware, membongkar sebuah program, dan dalam pembuatan sistem operasi.


Ada dua model CPU, CISC dan RISC.
CISC artinya Complex-Instruction-Set-Computer yang berarti satu instruksi bisa melakukan beberapa operasi.
RISC artinya Reduced-Instruction-Set-Computer dengan instruksi yang lebih sederhana dengan sedikit operasi namun tidak mengyampingkan kecepatan.

Register adalah tempat penyimpanan CPU. Kegunaan register ini diberikan dari penamaannya serta bagaimana ABI yang diterapkan.

## x86
x86 merupakan contoh arsitektur CPU yang sangat terkenal. 
Ia bertipe CISC dan sudah berevolusi sebanyak 3 kali: x86-16 (16 bit era DOS), x86-32 (32 bit, bisa disebut juga x86 atau i386), dan yang terakhir x86-64 (64 bit bisa disebut juga x64)

x86-64 memiliki 16 General Purpose Register

| Nama | Keterangan |
| --- | --- |
| `RAX` | Accumulator Register |
| `RCX` | Counter Register |
| `RDX` | Data Register |
| `RBX` | Base Register |
| `RSP` | Stack Pointer Register |
| `RBP` | Base Pointer Register |
| `RSI` | Source Index Register |
| `R8` - `R15` | - |

ABI adalah aturan bagaimana CPU digunakan termasuk mengatur bagaimana register-register tersebut digunakan.
Compiler C digunakan untuk memetakan kode C ke dalam kode Assembly.

Sebagai contoh, Windows menggunakan x64 ABI. 

| Return Value | arg0 | arg1 | arg2 | arg3 |
| --- | -- | -- | -- | -- |
| `RAX` | `RCX` | `RDX` | `R8` | R9` |

RAX digunakan untuk menyimpan nilai kembalian fungsi. `RCX` menyimpan argumen pertama, `RDX` menyimpan argumen kedua, `R8` menyimpan argumen ketiga, `R9` menyimpan argumen keempat.

Kita bisa lihat di sini https://godbolt.org/z/vjx38hcT8.

`RCX` menyimpan alamat dari string format `printf`, `RDX` menyimpan argumen kedua -1, dan seterusnya.

