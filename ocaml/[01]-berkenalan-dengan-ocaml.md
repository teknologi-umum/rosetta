---
title:  Berkenalan dengan OCaml
created: 28-07-2021
update: -
---

# 1. Berkenalan dengan OCaml

OCaml merupakan singkatan dari *Objective Categorial Abstract Machine Language*, sebuah bahasa pemrograman serba guna dan mendukung variasi paradigma (seperti, Imperatif, Berbasis-Objek dan Fungsional).

OCaml dapat berjalan di sistem operasi desktop seperti MacOS, Linux dan Windows (Dengan bantuan *chocolatey*), infomasi lebih lanjut ~~hubungi dokter~~ [disini](https://ocaml.org/learn/portability.html).


## Sejarah OCaml

Caml pertama kali di but pada tahun 1987 oleh Ascander Suarez yang dikembangkan sampai Tahun 1992, Caml dikembangkan oleh  [Pierre Weis](http://cristal.inria.fr/~weis/) and [Michel Mauny](http://cristal.inria.fr/~mauny/) karena kepergian Ascander pada tahun 1988. Kala itu Caml ditulis diatas LLM3 (mesin virtual dari sistem Le_Lisp).

Pada tahun 1990, [Xavier Leroy](http://cristal.inria.fr/~xleroy/) menulis impelmentasi Caml dalam bahasa C yang menjadi Caml Light.

Tahun 1995, [Xavier Leroy](http://cristal.inria.fr/~xleroy/) dan [Damien Doligez](http://cristal.inria.fr/~doligez/) membuat bahasa  pengembangan dari Caml Light yang diberi nama Caml Special Light dengan dukungan pembangkit *bytecode*. 

Seiring perkembanganya , Caml Special Light memiliki generator byte code yang lebih effisen, mengadopsi fitur StandardML. 

Seiring perkembangan dan penambahan fitur pada tahun 2010, Caml Special Light berganti nama menjadi OCaml dengan dukungan banyak paradigma seperti Imperatif, Berbasis Objek dan Fungsional.


## Bagaimana rupanya?

OCaml dapat di coba tanpa memasang kompiler secara online di [TryOCamlPro](https://try.ocamlpro.com/).

- Mencetak ke Konsol
	```ocaml
	let () = print_endline "Ora Bliding Ej, Ora Umum";;
	```
- Variabel
	```ocaml
	let nama = "Ayunda Mostovoy";;
	let () = print_endline("Hi, " ^ nama);;
	(* Hi, Ayunda Mostovoy *)
	```
- Pemilihan
	```ocaml
	let () = 
	  let kamu_orang = true and p = print_endline in
	  if kamu_orang then  p "Bukan Hantu" 
	  else if kamu_orang = false then p "Hantu"    
	  else  p "Hantu"
	;;
	```

- Perulangan
 Tidak ada while atau for hanya ada `loop` (infinite loop), fungsi rekursif dan iterator.

	```ocaml
	let () =
	  let kantong = [2;3;4;5;6;7;10] in
	  
	  (List.filter (fun y -> y mod 2 = 0) kantong)
	  |> List.iter print_int
	  |> ignore (* Membuang hasil List.iter*)
	;;
	```
- Fungsi
	```ocaml
	let sapa_dia (nama: string): string =
	  "Здравствуйте, " ^ nama 
	;;
	
	let () =
	  print_endline(sapa_dia("dari LaodeAI"))
	;;
	```
	- Kombinator fungsi (`|>`)
	
		Kombinator fungsi menyambungkan output dari suatu ekspresi akan menjadi input bagi ekspresi lain.
		```ocaml
		let tambah a b = a + b;;
		let kurang c d = c - d;;
		
		let () =
			(* print_int(kurang(tambah(1 2) 3)) *)
			2
			|> tambah 1
			|> kurang 3
			|> print_int
			;
		;;
		```
- Modul
	```ocaml
	module Contoh = struct
	  
	  let fungsi_modul = print_endline("Dari Dalam Modul") 

	end

	let () =
	  Contoh.fungsi_modul
	;;
	```
 
## Apa yang *Bliding Ej*  dari OCaml?

### Tipe Data Aljabar dan Pencocokan Pola

[WIP]

### Kompilasi ke *Native*

[WIP]

### Interop ke C

[WIP]

### Ekosistem yang kecil

OCaml tidak populer, ekosistem yang kecil dan banyak library yang cukup berumur tetapi masih bisa berjalan (*abandon but not obsolete*).  

Mesikpun salah satu pustaka besar seperti mirage (unikernel) memiliki banyak pustaka pembantu, namun adopsi komunitas lebih memilih membuat alternatif lain (*decision backslash*).

## Apakah bahasa ini dipakai dalam taraf produksi (*Production grade*)?
OCaml sudah dipakai dalam taraf produksi, contoh beberapa perusahaan yang menggunakan OCaml dalam platform nya : 
- [Jane Street](https://www.janestreet.com/technology/) 
- [Tarides](https://tarides.com/)
- [Tezos](https://tezos.com/)

