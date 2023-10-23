---
title: Berkenalan Dengan Bahasa Pemrogaman Go
created: 23-10-2023
update: -
---

## 1. Berkenalan Dengan Bahasa Pemrograman Go
Go merupakan bahasa pemrograman yang dibuat oleh search engine raksasa di masa ini, yaitu google, Go juga terkenal atau fitur yang paling mencolok adalah
fitur <b>concurrency</b> nya, Go juga dibuat diatas bahasa pemrograman C, dan Go juga memiliki garbage collection.

## 2. Sejarah Bahasa Pemrograman Go
Go dibuat pada tahun 2009, oleh Robert Griesemer, Rob Pike, dan Ken Thompson, semua dari tiga perancang bahasa tidak suka terhadap kompleksitas C++ sehingga menjadi motivasi utama untuk mendesain sebuah bahasa baru, Versi 1.0 di Go diluncurkan pada tahun 2012

## 3. Bagaimana Kode Go?
<li>Hello World</li>

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello World")
}
```

<li>Kondisi</li>

```go
package main

import "fmt"

func main() {
	nilai := 2

	if nilai >= 7 {
		fmt.Println("A")
	} else if nilai <= 6 && nilai >= 3 {
		fmt.Println("B")
	} else {
		fmt.Println("C")
	}
}
```

<li>Perulangan</li>

```go
package main 

import "fmt"

package main() {
	angka := 20
	
	for i := 0; i < angka; i++ {
		fmt.Println(i)
        }       
}

```

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
