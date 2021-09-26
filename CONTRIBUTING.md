## Kontribusi 

#### Standarisasi Penulisan

- Tambahkan materi secara terurut dan terstruktur.
- Aturan penamaan tutorial :
  - Aturan : `[0<nomor urut>]-[judul].md`
  - `[01]-pengenalan_ruby.md`
- Letakkan tutorial di folder dan tempat yang tepat:
  - misal : `/ruby/[01]-pengenalan_ruby.md`
- Tambahkan ke daftar isi agar mudah dicari pada berkas **README.md** , contohnya pada bagian **"Bahasa yang tersedia"** diatas.
- Tambahkan `main/[bahasa]/[0<nomor urut>]-[judul].md` ke [consume.json](./consume.json), jika kamu menambah topik baru pada bahasa/bahasa baru, nomor id berisi nomor urut dan susun sesuai nomor id.
- Akan lebih baik bila menggunakan format pesan *commit*, seperti ini
  - `[kata kerja]([bahasa]): [Pesan]`
  - `add(OCaml): menambahkan 04.Pattern Matching`
  - `remove(Javascript): menghapus bagian X di 03. Installasi Javascript`
  - `fix(Rust): Memperbaiki bagian X di 09. Ownership`
- Gunakan bahasa yang mudah dimengerti dan tidak mengandung kalimat tidak senonoh.

#### Langkah untuk Kontribusi

- _Fork_ Repo Ini
- _Clone_ hasil _fork_ repo ini ke local anda
- Tambahkan apa yang ingin Anda lakukan
- _Commit_
- _New Pull Request_
