## Objective
- [Paragraf](#paragraf)
- [Format Teks](#format-teks)
- [Heading](#heading)
- [Horizontal Line](#horizontal-line)
- [Komentar](#komentar)
- [Elemen HTML](#elemen-html)
- [Atribut HTML](#atribut-html)
- [Image](#image)
- [Link](#link)
- [List](#list)
- [Table](#table)
- [Inline dan Blok Elemen](#inline-dan-blok-elemen)
- [Form](#form)
- [HTML Color](#html-color)
- [Frame](#frame)

## Paragraf
### Tag `<p>`
Tag `<p></p>` digunakan untuk membuat sebuah paragraf
``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <p>Contoh paragraf 1</p>
    <p>Contoh paragraf 2</p>
  </body>
</html>
```

### Tag `<br/>`
Tag `<br/>` digunakan untuk menambahkan 1 line baru
``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <p>Contoh paragraf 1</p>
    <p>Contoh paragraf 2</p>
    <p>Contoh <br/> line break</p>
  </body>
</html>
```

## Format Teks
HTML memiliki beberapa elemen yang memberikan style pada teks.
``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <p>Teks biasa</p>
    <p><b>Bold teks</b></p>
    <p><big>Big teks</big></p>
    <p><i>Italic teks</i></p>
    <p><small>Small teks</small></p>
    <p><strong>Strong teks</strong></p>
    <p><sub>Subscript teks</sub></p>
    <p><sup>Superscript teks</sup></p>
    <p><ins>Insert teks</ins></p>
    <p><del>Delete teks</del></p>
  </body>
</html>
```

Output:

![alt text][format_teks]

## Heading
HTML memiliki 6 level heading yang dikelompokan berdasarkan kepentingan yakni `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>` dan `<h6>`
``` html
<html>
  <head>
    <title>Halaman pertama</title>
  </head>
  <body>
    <h1>Heading pertama</h1>
    <h2>Heading kedua</h2>
    <h3>Heading ketiga</h3>
    <h4>Heading keempat</h4>
    <h5>Heading kelima</h5>
    <h6>Heading keenam</h6>
  </body>
</html>
```

Output:

![alt text][heading]

> Tidak direkomendasikan untuk membuat teks bold dengan menggunakan heading dikarenakan search engine menggunakan heading sebagai index dari struktur dan konten halaman web.

## Horizontal Line
Tag `<hr/>` digunakan untuk membuat garis horizontal (horizontal line)
``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <h1>Heading pertama</h1>
    <h2>Heading kedua</h2>
    <h3>Heading ketiga</h3>
    <h4>Heading keempat</h4>
    <h5>Heading kelima</h5>
    <h6>Heading keenam</h6>
    <hr/>
    <p>Contoh paragraf</p>
  </body>
</html>
```

Output:

![alt text][horizontal_line]

## Komentar
Komentar tidak akan ditampilkan oleh browser. Komentar digunakan sebagai catatan atau deskripsi pada dokumen HTML.

``` html
<!-- Komentar disini -->
```

Contoh:
``` html
<!DOCTYPE html>
<html>
<head>
  <title>Halaman Pertama</title>
</head>
<body>
  <p>Contoh paragraf 1</p>
  <!-- Contoh komentar -->
  <p>Contoh paragraf 2</p>
  <!-- <p>Contoh paragraf 3</p> -->
</body>
</html>
```

Output:

![alt text][komentar]

## Elemen HTML
Dokumen HTML terbuat dari elemen-elemen HTML dan elemen HTML dituliskan menggunakan _tag awal_ dan _tag akhir_ dengan disisipkan konten diantara tag.
Beberapa elemen HTML tidak mempunyai _tag akhir_
``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <p>Contoh <br/> paragraf</p>
  </body>
</html>
```

## Atribut HTML
Atribut HTML menyediakan informasi tambahan mengenai sebuah elemen atau tag HTML dan juga digunakan untuk memodifikasi elemen atau tag tersebut.
``` html
<p align="center">
  Contoh teks ini akan berada ditengah
</p>

<hr width="50%">
<hr width="50px">
```

Untuk satuan suatu nilai ukuran dapat menggunakan px (pixel) atau % (persentase).

## Image
Tag `<img>` digunakan untuk memasukkan sebuah gambar. Tag ini hanya mempunyai atribut dan tidak mempunyai tag akhir.
URL dari gambar dapat didefinisikan dengan menggunakan atribut src.
``` html
<img src="gambar.jpg"/>
```

### Lokasi gambar
Lokasi gambar didefinisikan pada atribut src diantara tanda petik dua.

Contoh, jika mempunyai foto dengan nama "laptop.jpg" dan lokasi foto tersebut sama dengan lokasi dari file html maka kodenya akan seperti berikut ini:
``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <img src="laptop.jpg" alt=""/>
  </body>
</html>
```

Jika gambar tidak muncul maka atribut alt digunakan sebagai alternatif teks yang akan muncul untuk mendeskripsikan gambar yang tidak muncul. Atribut alt harus didefinisikan pada tag `<img>` (required).

### Mengubah Ukuran Gambar
Untuk mendefinisikan gambar dapat menggunakan atribut width dan height. Satuan nilai yang diberikan dapat dalam pixel atau persentase.
``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <img src="laptop.jpg" height="150px" width="150px" alt="" />
    <!-- or -->
    <img src="laptop.jpg" height="50%" width="50%" alt="" />
  </body>
</html>
```

> Proses memuat gambar membutuhkan waktu, semakin besar ukuran gambar maka semakin lama gambar dimuat.

### Border Gambar
Secara default, sebuah gambar tidak memiliki border. Atribut border digunakan untuk membuat sebuah border mengelilingi gambar tersebut.
``` html
<img src="laptop.jpg" height="150px" width="150px" border="1px" alt="" />
```

## Link
Tag `<a>` digunakan untuk membuat link pada dokumen HTML sehingga pada saat user mengklik suatu link akan terhubung ke dokumen HTML lainnya. Link dapat ditambahkan pada teks ataupun gambar.
``` html
<a href="http://github.com/tedydarmawan">View Github</a>
```

### Atribut target
Atribut target menentukan tempat untuk membuka link dokumen. Nilai `_blank` pada atribut target akan membuka link pada new window atau new tab.
``` html
<a href="http://github.com/tedydarmawan" target="_blank">View Github</a>
```

## List
List pada HTML terdiri dari dua macam yaitu Ordered List dan Unordered List.

### Ordered List
Ordered List dimulai dengan tag `<ol>` dan setiap item list didefinisikan dengan tag `<li>`
``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <ol>
      <li>Merah</li>
      <li>Kuning</li>
      <li>Hijau</li>
    </ol>
  </body>
</html>
```

Output:

![alt text][ordered_list]

### Unordered List
Sama halnya seperti ordered list hanya saja dimulai dengan tag `<ul>`
``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <ul>
      <li>Merah</li>
      <li>Kuning</li>
      <li>Hijau</li>
    </ul>
  </body>
</html>
```

Output:

![alt text][unordered_list]

## Table
Tag `<table>` digunakan untuk membuat table. Suatu tabel pasti memiliki row dan kolom. Untuk membuat row dapat menggunakan tag `<tr>` dan untuk membuat kolom dapat menggunakan tag `<td>` yang dapat berisi teks, gambar, list atau tabel lainnya.

Berikut ini contoh 1 row dan 3 kolom
``` html
<table>
  <tr>
    <td>Teks 1</td>
    <td>Teks 2</td>
    <td>Teks 3</td>
  </tr>
</table>
```

### Atribut Border, Colspan dan Rowspan
Untuk menambahkan border pada suatu tabel dapat menggunakan atribut border
``` html
<table border="2">
```

Suatu kolom tabel dapat memiliki 1 atau banyak kolom. Untuk itu dapat menggunakan atribut colspan
``` html
<table border="2">
  <tr>
    <td>Merah</td>
    <td>Kuning</td>
    <td>Hijau</td>
  </tr>
  <tr>
    <td>Biru</td>
    <td colspan="2">Jingga</td>
  </tr>
</table>
```

Output:

![alt text][border_colspan]

Suatu row tabel dapat memiliki 1 atau banyak row. Untuk itu dapat menggunakan atribut rowspan
``` html
<table border="2">
  <tr>
    <td rowspan="2">Merah</td>
    <td>Kuning</td>
    <td>Hijau</td>
  </tr>
  <tr>
    <td>Biru</td>
    <td>Jingga</td>
  </tr>
</table>
```

Output:

![alt text][border_rowspan]


[horizontal_line]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18836053_10212785244096548_7943358643832976492_n.jpg?oh=ba3ef1a6cb16957e3240a7faebeff2ee&oe=59E3F697 "Horizontal Line"
[format_teks]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18882129_10212785247816641_7604391083173436618_n.jpg?oh=629743a6a15aed30c83423dec84765d8&oe=59AC0D58 "Format Teks"
[heading]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18920581_10212785247896643_2860304077462280781_n.jpg?oh=629887972afa8b427fbfe40c7737fdee&oe=59A3B171 "Heading"
[komentar]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18921824_10212785313538284_4475550903791816041_n.jpg?oh=2f11e6e5eb9c1806f5f9e528dc3e19ae&oe=59E0EBF7 "Komentar"
[ordered_list]: https://scontent.fcgk8-1.fna.fbcdn.net/v/t1.0-9/18920209_10212785877632386_8597960058524977492_n.jpg?oh=fd90ee1134a9f4450ee5880bbe8981d5&oe=59AABF48 "Ordered List"
[unordered_list]: https://scontent.fcgk8-1.fna.fbcdn.net/v/t1.0-9/18835514_10212785877712388_1171053387322764886_n.jpg?oh=431c905570ae90cbc36e3f11c1e7dcf0&oe=59E9E922 "Unordered List"
[border_colspan]: https://scontent.fcgk8-1.fna.fbcdn.net/v/t1.0-9/18920680_10212785960834466_1963298013341911394_n.jpg?oh=22b7855fda8e0a19253503b178c4247c&oe=59DD2738 "Border Colspan"
[border_rowspan]: https://scontent.fcgk8-1.fna.fbcdn.net/v/t1.0-9/18922222_10212785989915193_3087695514612876468_n.jpg?oh=61dc21929f8621f4d99590d63bb4a6ae&oe=59E1AF77 "Border Rowspan"
