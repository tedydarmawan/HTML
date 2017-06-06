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
- [Elemen Inline dan Blok](#elemen-inline-dan-blok)
- [Form](#form)
- [HTML Color](#html-color)

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

### Atribut align dan bgcolor
Tag align digunakan untuk mengatur posisi dari tabel.
``` html
<table align="center">
```

Tag bgcolor digunakan untuk mewarnai tabel, row atau kolom
```
<table border="2" align="center">
  <tr>
    <td bgcolor="red">Merah</td>
    <td>Kuning</td>
    <td>Hijau</td>
  </tr>
  <tr>
    <td>Biru</td>
    <td>Jingga</td>
    <td>Ungu</td>
  </tr>
</table>
```

Output:

![alt text][bgcolor_align]

## Elemen Inline dan Blok
Pada HTML, sebagian besar elemen didefinisikan sebagai elemen blok atau elemen inline.

### Elemen Blok
Elemen blok dimulai dari line baru, contohnya: `<h1>`, `<form>`, `<li>`, `<ol>`, `<ul>`, `<p>`, `<pre>`, `<table>`, `<div>` dan lainnya.

Tag `<div>` sering digunakan sebagai container untuk elemen-elemen HTML lainnya. Ketika digunakan bersamaan dengan CSS, tag `<div>` dapat digunakan untuk membuat style blok konten.

``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <h1>Judul</h1>
    <div style="background-color: blue; color: white; padding: 20px;">
      <p>Paragraf pertama</p>
      <p>Paragraf kedua</p>
    </div>
  </body>
</html>
```

Output:

![alt text][div]

### Elemen Inline
Elemen inline biasanya ditampilkan tanpa jeda baris, contohnya: `<b>`, `<a>`, `<strong>`, `<img>`, `<input>`, `<em>`, `<span>` dan lainnya.

Tag `<span>` yang merupakan elemen inline sering digunakan sebagai container untuk teks. Ketika digunakan bersamaan dengan CSS, tag `<span>` dapat digunakan untuk membuat style untuk beberapa bagian teks.

``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <h2>Beberapa Pesan <span style="color: red;">Penting!</span></h2>
  </body>
</html>
```

Output:

![alt text][span]

> Elemen blok dapat berisi beberapa elemen inline tetapi tidak sebaliknya elemen inline tidak dapat berisi elemen blok

## Form
Form pada HTML biasanya digunakan untuk memperoleh informasi dari user. Form didefinisikan dengan tag awal `<form>` dan tag akhir `</form>`.
``` html
<body>
  <form>
    <!-- elemen input form disini-->
  </form>
</body>
```

### Atribut action
Gunakan atribut action untuk memuat halaman web sesudah user melakukan submit form.
``` html
<form action="http://www.github.com/tedydarmawan">
</form>
```

### Atribut method
Atribut method menentukan method HTTP (GET atau POST) yang digunakan ketika form disubmit.
``` html
<form action="http://www.github.com/tedydarmawan" method="GET">

<!-- atau -->

<form action="http://www.github.com/tedydarmawan" method="POST">
```

> Ketika menggunakan GET, pada saat submit, data pada form akan terlihat di alamat web atau URL. POST digunakan jika form dibuat untuk mengupdate data atau berisi informasi sensitif seperti password. POST memiliki security yang lebih baik karena data yang disubmit tidak terlihat di alamat web atau URL.

### Atribut name
Atribut name digunakan untuk menentukan nama dari suatu elemen input pada form. Untuk mengambil inputan user diperlukan elemen input form seperti text, radio dan lainnya.

Berikut ini contoh form untuk mendapatkan username dan password
``` html
<form>
  <input type="text" name="username" /><br />
  <input type="password" name="password" />
</form>
```

Output:

![alt text][form_name]

### Elemen Input pada Form

#### Radio
Jika input type diubah menjadi radio maka user hanya dapat memilih salah satu dari beberapa pilihan.
``` html
<input type="radio" name="gender" value="1" />Lelaki<br />
<input type="radio" name="gender" value="2" />Perempuan<br />
```

Output:

![alt text][radio]

#### Checkbox
Input type checkbox membuat user dapat memilih beberapa pilihan (lebih dari 1)
``` html
<input type="checkbox" name="gender" value="1" />Lelaki<br />
<input type="checkbox" name="gender" value="2" />Perempuan<br />
```

Output:

![alt text][checkbox]


#### Submit
Input type submit digunakan untuk membuat button yang akan mentrigger aksi dari atribut action pada form
``` html
<input type="submit" value="Submit" />
```

Output:

![alt text][submit]

Setelah disubmit data akan diproses oleh backend.

## HTML Color
HTML Color atau warna pada HTML diekspresikan dalam nilai heksadesimal: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F. Nilai 0 merepresentasikan nilai terkecil dan F merepresentasikan nilai terbesar.

Warna pada HTML ditampilkan dalam kombinasi red, green and blue (RGB).
Nilai heksadesimal dituliskan menggunakan simbol hashtag (#) diikuti dengan 3 atau 6 karakter heksadesimal.

``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body bgcolor="#FF0000">
    <font color="#FFFFFF">Headline Warna Putih</font>
  </body>
</html>
```

Output:

![alt text][color]


[horizontal_line]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18836053_10212785244096548_7943358643832976492_n.jpg?oh=ba3ef1a6cb16957e3240a7faebeff2ee&oe=59E3F697 "Horizontal Line"
[format_teks]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18882129_10212785247816641_7604391083173436618_n.jpg?oh=629743a6a15aed30c83423dec84765d8&oe=59AC0D58 "Format Teks"
[heading]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18920581_10212785247896643_2860304077462280781_n.jpg?oh=629887972afa8b427fbfe40c7737fdee&oe=59A3B171 "Heading"
[komentar]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18921824_10212785313538284_4475550903791816041_n.jpg?oh=2f11e6e5eb9c1806f5f9e528dc3e19ae&oe=59E0EBF7 "Komentar"
[ordered_list]: https://scontent.fcgk8-1.fna.fbcdn.net/v/t1.0-9/18920209_10212785877632386_8597960058524977492_n.jpg?oh=fd90ee1134a9f4450ee5880bbe8981d5&oe=59AABF48 "Ordered List"
[unordered_list]: https://scontent.fcgk8-1.fna.fbcdn.net/v/t1.0-9/18835514_10212785877712388_1171053387322764886_n.jpg?oh=431c905570ae90cbc36e3f11c1e7dcf0&oe=59E9E922 "Unordered List"
[border_colspan]: https://scontent.fcgk8-1.fna.fbcdn.net/v/t1.0-9/18920680_10212785960834466_1963298013341911394_n.jpg?oh=22b7855fda8e0a19253503b178c4247c&oe=59DD2738 "Border Colspan"
[border_rowspan]: https://scontent.fcgk8-1.fna.fbcdn.net/v/t1.0-9/18922222_10212785989915193_3087695514612876468_n.jpg?oh=61dc21929f8621f4d99590d63bb4a6ae&oe=59E1AF77 "Border Rowspan"
[bgcolor_align]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18893067_10212792960649457_993785844553910840_n.jpg?oh=96da0a12c96eb7240eca7502663d8106&oe=59AA20A0 "bgcolor align"
[div]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18838990_10212793047651632_1235506268864750783_n.jpg?oh=7e2db0b7ebd39499ec04701d9ac1af2c&oe=59AA5482 "div"
[span]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18813521_10212793078132394_1321873764958248156_n.jpg?oh=666ae750ed48c1893de544db798bd692&oe=59ACFADB "span"
[form_name]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18839330_10212793222616006_253131349086428437_n.jpg?oh=3bcc06b7be6ebcd4dc2a7bec28497ada&oe=59E7EC84 "Form dengan atribut name"
[checkbox]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18838931_10212793353459277_5577384524749670963_n.jpg?oh=06942b5df780fa063dd4bb5ae556027d&oe=59AF8B9D "Checkbox"
[radio]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/19030193_10212793353419276_4994530983937859812_n.jpg?oh=2c23649ccf250ff1baceb076516b98f7&oe=59E1669C "Radio"
[submit]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18839097_10212793389500178_6815866475479269412_n.jpg?oh=c6a1e2bc09a52fcbf985f1eca97d4e8d&oe=59ADFB53 "Submit"
[color]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18950986_10212793437701383_6285407354061500417_n.jpg?oh=131375e988a01673dfb517bcea20b4ce&oe=59A4C38B "HTML Color"
