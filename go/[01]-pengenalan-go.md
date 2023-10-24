---
title: Berkenalan Dengan Bahasa Pemrograman Go
created: 23-10-2023
update: -
---

## Instalasi Go
Anda bisa install Go (Golang) di web official nya [disini](https://go.dev/dl).</br>
Lalu lakukan install seperti biasa, jika dirasa sudah terinstall jalankan command ```go version```. Maka akan muncul versi golang yang kamu install.

## 1. Berkenalan Dengan Bahasa Pemrograman Go
Go merupakan bahasa pemrograman yang dibuat oleh search engine raksasa di masa ini, yaitu Google, Go juga terkenal atau fitur yang paling mencolok adalah
fitur <b>concurrency</b> nya, Go juga dibuat diatas bahasa pemrograman C, dan Go juga memiliki garbage collection.

## 2. Sejarah Bahasa Pemrograman Go
Go dibuat pada tahun 2009, oleh Robert Griesemer, Rob Pike, dan Ken Thompson, semua dari tiga perancang bahasa tidak suka terhadap kompleksitas C++ sehingga menjadi motivasi utama untuk mendesain sebuah bahasa baru, Go versi 1.0 diluncurkan pada tahun 2012.

## 3. Bagaimana Kode Go?
Sebelum kamu ikut di tutorial ini kamu sudah harus menginstall Go di device yang kamu gunakan</br></br>
Lalu buat folder bernama <b>Belajar Go</b>, dan buka terminal/cmd kamu dan jalankan command ```go mod init belajar-go```.
<li>Hello World</li>

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello World")
}
```
Tulis kode diatas di dalam file```main.go```.</br>
Lalu jalankan command ini:
```bash
go run main.go
```

<b>Output:</b>
```text
Hello World
```

<li>Kondisi</li>

```go
package main

import "fmt"

func main() {
	nilai := 10

	if nilai >= 7 {
		fmt.Println("A")
	} else if nilai <= 6 && nilai >= 3 {
		fmt.Println("B")
	} else {
		fmt.Println("C")
	}
}
```

Tulis kode diatas di dalam file```main.go```.</br>
Lalu jalankan command ini:
```bash
go run main.go
```

<b>Output:</b>
```text
A
```

<li>Perulangan</li>

```go
package main 

import "fmt"

package main() {
	angka := 5
	
	for i := 0; i < angka; i++ {
		fmt.Println(i)
        }       
}

```
Tulis kode diatas di dalam file```main.go```.</br>
Lalu jalankan command ini:
```bash
go run main.go
```

<b>Output:</b>
```text
0
1
2
3
4
```

Mengapa 5 tidak muncul? karena 5 tidak dibawah 5, Simple, jika ingin angka 5 muncul, maka ganti ```i < angka``` menjadi ```i <= angka```.


<li>Function</li>

```go
package main

import "fmt"

func sayHello(name string) {
	fmt.Println("Hello ", name)
}

func main() {
	name := "Refaldy"
	
	sayHello(name)
}
```

Tulis kode diatas di dalam file```main.go```.</br>
Lalu jalankan command ini:
```bash
go run main.go
```

<b>Output:</b>
```text
Hello Refaldy
```

### Penjelasan Kode Go
Kita sudah menulis dan mencoba kode Go dasar diatas, maka izinkan saya menjelaskan apa isi dari kode tersebut.

<li>package main</li>

Pada kode diatas selalu , menuliskan ```package main```, mengapa?
Karena simplenya Dalam bahasa pemrograman Go (Golang), penamaan paket sebagai "main" memiliki makna khusus. Paket dengan nama "main" digunakan sebagai paket utama atau entry point program.

<li>import "fmt"</li>

keyword ```import``` untuk mengimport package std maupun luar.

<li>func main()</li>

Di Go (Golang), setiap program harus memiliki fungsi ```main``` sebagai titik masuk utama atau entry point dari program. Hal ini wajib ada karena ```main``` adalah fungsi yang akan dieksekusi pertama kali ketika program dijalankan
