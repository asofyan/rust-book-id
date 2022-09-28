# Bahasa Pemrograman Rust

![Build Status](https://github.com/rust-lang/book/workflows/CI/badge.svg)

Repositori ini berisi sumber buku "Bahasa Pemrograman Rust".

[Buku ini tersedia dalam format dead-tree dari No Starch Press][nostarch].

[nostarch]: https://nostarch.com/rust

Anda juga dapat membaca buku ini secara daring dan gratis. Mohon dicek buku yang dilengkapi dengan
rilis Rust terbaru versi [stable], [beta], atau [nightly]. Perhatikan bahwa masalah
di versi tersebut sudah diperbaiki di dalam repositori, mengingat rilis tersebut diperbarui lebih jarang

[stable]: https://doc.rust-lang.org/stable/book/
[beta]: https://doc.rust-lang.org/beta/book/
[nightly]: https://doc.rust-lang.org/nightly/book/

Lihat bagian [releases] untuk mengunduh semua kode yang digunakan di dalam buku ini.

[releases]: https://github.com/rust-lang/book/releases

## Persyaratan

Untuk membuat buku ini perlu [mdBook], idealnya dalam versi yang sama dengan yang digunakan 
rust-lang/rust dalam [berkas ini][rust-mdbook]. Untuk mendapatkannya:

[mdBook]: https://github.com/rust-lang-nursery/mdBook
[rust-mdbook]: https://github.com/rust-lang/rust/blob/master/src/tools/rustbook/Cargo.toml

```bash
$ cargo install mdbook --vers [version-num]
```

## Pembuatan

Untuk membuat buku, ketik:

```bash
$ mdbook build
```

Keluarannya akan tersimpan dalam sub direktori `book`. Untuk mengeceknya, buka dengan peramban.

_Firefox:_
```bash
$ firefox book/index.html                       # Linux
$ open -a "Firefox" book/index.html             # OS X
$ Start-Process "firefox.exe" .\book\index.html # Windows (PowerShell)
$ start firefox.exe .\book\index.html           # Windows (Cmd)
```

_Chrome:_
```bash
$ google-chrome book/index.html                 # Linux
$ open -a "Google Chrome" book/index.html       # OS X
$ Start-Process "chrome.exe" .\book\index.html  # Windows (PowerShell)
$ start chrome.exe .\book\index.html            # Windows (Cmd)
```

Untuk menjalankan tests:

```bash
$ mdbook test
```

## Kontribusi

Kami sangat menyukai bantuan Anda! Mohon lihat [CONTRIBUTING.md][contrib] untuk mengetahui
kontribusi apa saja yang kami butuhkan.

[contrib]: https://github.com/rust-lang/book/blob/main/CONTRIBUTING.md

Karena buku ini [dicetak](https://nostarch.com/rust), dan karena kami ingin 
menjaga sebisa mungkin versi daring sama dengan versi cetak, setiap Anda mengajukan _issue_
atau _pull request_, tanggapan kami menjadi lebih lama.

Sejauh ini, kami telah merevisi lebih banyak agar sesuai dengan [Edisi Rust](https://doc.rust-lang.org/edition-guide/). 
Di antara revisi besar tersebut, kami hanya memperbaiki _error_. Jika _issue_ atau _pull request_ Anda
tidak secara khusus memperbaiki kesalahan (_error_) maka isu itu akan tetap di sana hingga kami bekerja
di dalam versi yang lebih besar: diperkirakan dalam hitungan bulan atau tahun.
Terima kasih atas kesabaran Anda! 

### Terjemahan

Kami menyukai semua bantuan penerjemahan buku! Lihat label [Translations] untuk bergabung dalam upaya penerjemahan
yang saat ini masih berjalan. Bukalah isu baru untuk mulai bekerja dalam bahasa yang baru!
Kami tunggu dalam [mdbook support] untuk dukungan multi bahasa sebelum kami menggabungkannya, tapi silakan mulai kapan saja!

[Translations]: https://github.com/rust-lang/book/issues?q=is%3Aopen+is%3Aissue+label%3ATranslations
[mdbook support]: https://github.com/rust-lang-nursery/mdBook/issues/5

## Cek Ejaan

Untuk memindai berkas sumber salah eja, Anda bisa gunakan skrip `spellcheck.sh`
yang tersedia di direktori `ci`. Pengecekan salah eja butuh kata-kata valid,
yang bisa ditemukan di `ci/dictionary.txt`. Jika skrip mengeluarkan _false
positive_ (seharusnya benar tapi dianggap salah, misalnya kata `BTreeMap` yang menurut skrip tidak valid),
Anda harus menambahkan kata tersebut ke dalam `ci/dictionary.txt` (mohon dijaga urutannya untuk menjaga konsistensi).
