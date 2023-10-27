---
title: Statement If Else
created: 27-10-2023
update: -
---

## Statement If Else Di Go

### Apa itu statement `if`?
Pernyataan `if` digunakan untuk melakukan pengujian kondisi tertentu dan menjalankan blok kode jika kondisi tersebut benar `(true)`.
<br><br>
Contoh:
```go
if condition {
    // do something in here
}
```

Contoh Penggunaan:
```go
package main

import "fmt" //Import package fmt

func main() {
    x := 10 //Deklarasi variable `x` dengan value 10

    if x > 5 { //Buat statement if, jika x lebih besar dari 5
        fmt.Println("Nilai x lebih besar dari 5") //Jika statement tersebut benar (true), maka akan mencetak "Nilai x lebih besar dari 5"
    }
}

//Output: Nilai x lebih besar dari 5
```
### Apa statement `if` `else` dalam Go
Pernyataan `if` `else` digunakan untuk menjalankan satu blok kode jika kondisi benar `(true)` dan blok kode lain jika kondisi salah `(false)`.<br><br>
Contoh:
```go
if condition {
    // Jalankan jika kondisi benar (true)
} else {
    // Jalankan jika kondisi salah (false)
}
```
Contoh Penggunaan:
```go
package main

import "fmt" //Import package fmt

func main() {
    x := 3 //Deklarasi variable x dengan value 3

    if x > 5 { //Buat pernyataan if, jika nilai x lebih besar dari 5
        fmt.Println("Nilai x lebih besar dari 5") //Jika x lebih besar dari 5 maka jalankan blok kode berikut.
    } else { //Jika pernyataan if tersebut salah (false), maka jalankan blok kode dibawah.
        fmt.Println("Nilai x kurang dari atau sama dengan 5") //Jika hasil dari pernyataan if adalah salah (false), maka jalankan kode ini.
    }
	
	//Output: Nilai x kurang dari atau sama dengan 5.
}
```
### Pernyataan `if` `else if` dalam Golang
Pernyataan `if` `else if` digunakan untuk menguji beberapa kondisi berurutan dan menjalankan blok kode yang sesuai dengan kondisi yang pertama yang benar `(true)`.

Contoh:
```go
if condition1 {
    // Jalankan jika kondisi1 benar (true)
} else if condition2 {
    // Jalankan jika kondisi2 benar (true)
} else {
    // Jalankan jika semua kondisi salah (false)
}
```

Contoh Penggunaan:
```go
package main

import "fmt"

func main() {
    x := 7 //Deklarasi variable x dengan value 7

    if x > 10 { //buat pernyataan if, jika nilai x lebih dari 10.
        fmt.Println("Nilai x lebih besar dari 10") //Jika pernyataan `if` bernilai `true`, maka jalankan kode berikut
    } else if x > 5 { // Jika nilai x lebih besar dari 
        fmt.Println("Nilai x lebih besar dari 5 tetapi kurang dari atau sama dengan 10") //jika pernyataan `else if` bernilai `true` maka jalankan kode berikut.
    } else { //Buat pernyataan `else` Jika pernyataan `if` dan `else if` bernilai salah (false).
        fmt.Println("Nilai x kurang dari atau sama dengan 5")
    }
	
	//Output:  Nilai x lebih besar dari 5 tetapi kurang dari atau sama dengan 10
}
```