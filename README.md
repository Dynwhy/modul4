##### Nama = Dio Firmansyah
##### kelas = XII RPL 1 / 22
# Modul4

sebelum lanjut, buka dulu modul 3 sebelum melakukan modul 4 
pertama bikin folder pada views beserta di VSCode:
### folder dan file
- barang
 ==> nama filenya > home.blade.php
- kategori
==> nama filenya >  index.blade.php
- layout
==> nama filenya >  app.blade.php

seperti gambar dibawar ini

![image](https://user-images.githubusercontent.com/109930420/183367954-62b56cad-d9a1-47cc-b965-70a1fa933336.png)

>Tugas 2 membuat layout dengan master template blade untuk project anda
langkah ke dua pada folder layout `file app.blade.php` kita mengambil **css dan js di bootstrap** ini linknya
[Bootstrap](https://getbootstrap.com/docs/5.2/getting-started/introduction/)
atau seperti foto di bawah

![image](https://user-images.githubusercontent.com/109930652/183359409-e28f5e85-dff5-4566-ab1d-cbb1857bbcd6.png)

menambahkan syntax sebagai berikut pada `app.blade.php`
```
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css">
```

selanjutnya bagian js dengan menambahkan syntax sebagai berikut pada `app.blade.php`
```
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.bundle.min.js"></script>
```

hasil salinan dibawah ini dan `app.blade.php` dengan all codenya

*periksa dengan teliti

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <link rel= "stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css">
    <title>
        @yield('title')
    </title>
</head>
<body>
    <!-- untuk navbar  -->
    <div class="container">
    <nav class="navbar navbar-expand-lg bg-dark">

  <div class="container-fluid">
    <a class="navbar-brand text-white" href="#">penjualan</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active text-white" aria-current="page" href="/">home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-white" href="/kategori">kategori</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-white" href="/barang">barang</a>
        </li>
</div>

</div>
</nav>
</div>
<div class = "container">
    @yield('content')
</div>
 <script src="httpscdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.bundle.min.js"></script>   
</body>
</html>
```
selanjutnya kita akan masukan script seperti dibawa ini, pada file `home.blade.php` di folder `barang` yang kita buat tadi
```
@extends ('layout.app')

@section('title')
barang
@endsection

@section('content')
<div class="mt-3">
<table class="table table-stripet">
        <thead>
            <tr>
                <th width="5%"> No.</th>
                <th>Nama</th>
                <th width ="15%">Kategori</th>
                <th width ="10%">Qty</th>
                <th width ="15%">Harga Beli</th>
                <th width ="15%">Harga Jual</th>
                <th width ="15%">Aksi</th>
</tr>
</thead>

<tbody>
    <tr>
        <td>1</td>
        <td>Meja</td>
        <td>ATK</td>
        <td>1</td>
        <td>50000</td>
        <td>55000</td>
        <td>Hapus | Edit</td>
</tr>
</tbody>
</table>
</div>
@endsection
```

selanjutnya kita akan masukan script pada file `index.blade.php` di folder `kategori` yang kita buat tadi
```
@extends ('layout.app')

@section('title')
Kategori
@endsection
@section('content')
<div class="mt-3">
    <table class="table table-stripet">
        <thead>
            <tr>
                <th width="5%"> No.></th>
                <th>Nama</th>
                <th width = "15%">Aksi</th>
</tr>
</thead>

<tbody>
    <tr>
        <td>1</td>
        <td>ATK</td>
        <td>Hapus|Edit</td>
</tr>
</tbody>
</table>
</div>
@endsection
```
hasil dari code yang kita kerjakan akan terlihat seperti dibawah ini

code yang ditampilkan ini dari folder barang file `home.blade.php`

![image](https://user-images.githubusercontent.com/109930652/183362035-7387b5b9-f680-431b-9d38-ad2f9313a50f.png)

lalu hasil folder kategori file `index.blade.php`

![image](https://user-images.githubusercontent.com/109930652/183362284-61fa8fad-6ac2-4dcd-9181-4a6e3f6c6fc5.png)

# Selesailah modul 4

## *SEMISAL ADA YANG EROR COBA LEBIH TELITI LAGI YAA:3
# SEKIAN TERIMA KASIH>.<
