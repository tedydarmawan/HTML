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



[horizontal_line]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18836053_10212785244096548_7943358643832976492_n.jpg?oh=ba3ef1a6cb16957e3240a7faebeff2ee&oe=59E3F697 "Horizontal Line"
[format_teks]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18882129_10212785247816641_7604391083173436618_n.jpg?oh=629743a6a15aed30c83423dec84765d8&oe=59AC0D58 "Format Teks"
[heading]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18920581_10212785247896643_2860304077462280781_n.jpg?oh=629887972afa8b427fbfe40c7737fdee&oe=59A3B171 "Heading"
[komentar]: https://scontent.fcgk9-1.fna.fbcdn.net/v/t1.0-9/18921824_10212785313538284_4475550903791816041_n.jpg?oh=2f11e6e5eb9c1806f5f9e528dc3e19ae&oe=59E0EBF7 "Komentar"
