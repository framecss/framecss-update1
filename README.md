[<img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhKljx6UhgoG9JxlJzKsxkNjBEzu8Xe6HUcpz6Xdw9cWSx1n-R6fM2HVstqb8FA3FxA7JU-NnEOHKChDNi3VHo8IvodX5erfcRcTztr6s3r7bj4cn02B6q6X6L1S6f2F2BkrRhtVUyTyvekJknoJ7u34PXPzrSH4K1Gq7om86iuUs1NTL-V23Mf_IVtag/s4096/framecss-1-1.jpg" width=55%>](https://github.com/nelsenpro/frame)
# Selamat Datang di ::Framecss Framework CSS
Menyediakan berbagai macam library CSS untuk keperluan Desain Aplikasi Web dan Website
# Download dan install 
### Terminal, Git, CMD : "git clone https://github.com/nelsenpro/frame.git"
### unduh versi 1.1.23 Alpha via [Github](https://github.com/nelsenpro/frame/archive/refs/heads/main.zip)
### unduh Versi 2.1.23 Alpha via [Github](https://github.com/nelsenpro/frame/raw/main/framecss/2.1.23.Alpha/framecss-2.alpha.zip)
| Nama | Deskripsi |
| --- | --- |
| Versi | 1.1.23 Alpha ; 1.2.23 Alpha| 
| Lisensi | GNU GPL 3 |
## Daftar isi :
- [Dokumentasi](#dokumentasi)
- [Struktur Framecss](#struktur-framecss)
- [Layout](#float-layout)
- [Grid Layout](#grid-layout)
- [Bikin Header](#membangun-header)
- [Bikin Panel](#membangun-panel)
- [Bikin Tombol](#membangun-tombol)
- [Bikin Tabel](#membangun-tabel)
- [Dokumentasi Lainnya](https://github.com/nelsenpro/frame/blob/main/framecss/2.1.23.Alpha/dokumentasi.md)
- [Creators](#creators)
- [Thanks](#thanks)
# Dokumentasi
## Struktur Framecss 
  ```text
framecss-2.alpha/
├── data/
│ ├── animate.css
│ ├── base.css
│ ├── fonts/
│ │
│ │
│ ├── frame.css
│ ├── frame.js
│ ├── gambar/
│ └── normalize.css
├── index.html
├── modif.css
└── modif.js
  ```
## Template Standar::Framecss
### Float Layout
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
            <!-- awal koneksi framecss -->
    <link rel="stylesheet" href="data/frame.css" type="text/css" media="all" />
            <!-- akhir koneksi framecss -->
    <title>Frame-CSS.1.Alpha</title>
</head>
<body>
    <div>
        <!-- bagian navbar-->
        <div class="" id="">
        <!-- akhir navbar-->
        
        <!-- bagian header, jumbotron- blok-->
        </div>
        <div class="">
            <h1 class="">Halo Dunia</h1>
            <p>
                ........
            </p>
        </div>
         <!-- akhir blok, jumbotron-->
         
         <!-- isi konten 1-->
        <div class="baris">
                <div class="utama samping">
                    <h2 class=""></h2>
                    <p></p>
                    <h2 class=""></h2>
                    <p></p>
                </div>
             <!-- akhir konten 1-->
             
             <!-- isi konten 2-->
                <div class="utama tengah">
                    <h2 class=""></h2>
                    <p></p>
                    <h2 class=""></h2>
                    <p></p>
                </div>
             <!-- akhir konten 2-->
             
             <!-- awal footer-->
        </div>
        <div class="kaki">
            <p class=""></p>
        </div>
           <!-- akhir footer-->
    </div>
        <!-- koneksi ke JavaScript-->
    <script src="data/frame.js"></script>
    <script src="modif.js"></script>
          <!-- akhir koneksi JavaScript-->
</body>
</html>
```
### Grid Layout
#### Grid 2 items
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="data/frame.min.css" type="text/css" media="all" />
    <title>Document</title>
</head>
<body>
    <div class="framecss-grid2">
        <div class="kepala">
            <h2>Kepala</h2>
        </div>

        <div class="badan-kiri">
            Badan Kiri
        </div>
        <div class="badan-tengah">
            Badan Tengah
        </div>

        <div class="kaki">
            <p>
                Kaki
            </p>
        </div>
    </div>
</body>
</html>
```
#### Grid 3 items
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="data/frame.min.css" type="text/css" media="all" />
    <title>framecss</title>
</head>
<body class="putih framecss">
    <div class="framecss-grid">
       <div class="kepala">
           <h1 class="hitam">Selamat Datang di Framecss Indonesia</h1>
           <small class="hitam">
               versi <i>2.1.23</i> <b>Alpha</b> 
           </small>
       </div>
       <div class="badan-kiri lbs-hijau">
           <div class="">
               <h2 class="">badan samping</h2>
           </div>
       </div>
       <div class="badan-tengah lbs-oren">
           <div class="">
               <h2 class="">badan tengah</h2>
           </div>
       </div>
       <div class="badan-kanan lbs-merah">
           <div class="">
               <h2 class="">badan kanan</h2>
           </div>
       </div>
       <div class="kaki">
           <h2 class="hitam">Kaki</h2>
       </div>
    </div>
</body>
</html>
```
## Membangun Header
### Header Navigasi 
```html
 <div class="nav" id="nav">
            <a href="#home" class="active">Beranda</a>
            <a href="#berita">Berita</a>
            <a href="#contact">Hubungi</a>
            <a href="#about">Tanya</a>
            <a href="#unduh">Unduh</a>
            <a href="#contoh">Contoh</a>
            <a href="javascript:void(0);" class="icon" onclick="navFunction()">
                <i class="fa fa-bars"></i>
            </a>
        </div>
```
```html
<div class="nav-hijau" id="nav-hijau">
            <a href="#home" class="active">Beranda</a>
            <a href="#news">Berita</a>
            <a href="#contact">Hubungi</a>
            <a href="#about">Tanya</a>
            <a href="#unduh">Unduh</a>
            <a href="#contoh">Contoh</a>
            <a href="javascript:void(0);" class="icon" onclick="hijauFunction()">
                <i class="fa fa-bars"></i>
            </a>
        </div>
```
### Header Panel
## Membangun Header Panel
### Panel Default
```html
<div class="kepala">
           <h1 class="hitam">Selamat Datang di Framecss Indonesia</h1>
           <small class="hitam">
               versi <i>2.1.23</i> <b>Alpha</b> 
           </small>
       </div>
```
### Panel modifikasi Latar 
```html
<div class="nav-ping" id="nav-ping">
            <a href="#home" class="active">Beranda</a>
            <a href="#news">Berita</a>
            <a href="#contact">Hubungi</a>
            <a href="#about">Tanya</a>
            <a href="#unduh">Unduh</a>
            <a href="#contoh">Contoh</a>
            <a href="javascript:void(0);" class="icon" onclick="pingFunction()">
                <i class="fa fa-bars"></i>
            </a>
        </div>
```
### Panel modifikasi Latar Animasi 
```html
 <div class="nav-kuning animasi-latar" id="nav-kuning">
            <a href="#home" class="active">Beranda</a>
            <a href="#berita">Berita</a>
            <a href="#contact">Hubungi</a>
            <a href="#about">Tanya</a>
            <a href="#unduh">Unduh</a>
            <a href="#contoh">Contoh</a>
            <a href="javascript:void(0);" class="icon" onclick="kuningFunction()">
                <i class="fa fa-bars"></i>
            </a>
        </div>
```
## Membangun Tombol
### tombol default 
```html
<button class="tombol" type="submit">Tombol</button>
```
### tombol modifikasi
```html
<button class="tombol bayang-merah u10px" type="submit">Tombol</button>
            <button class="tombol-kuning r12px" type="submit">Tombol</button>
            <button class="tombol-ping r8px bayang" type="submit">Tombol</button>
            <button class="tombol-magenta u25px bayang-hijau" type="submit">Tombol</button>
```
### tombol grup : Float pakai section, grid pakai div
```html
<section class="grup-tmb" style="width:">
                <button class="r12px frame expand" judul="tombol ini radius 12px" onclick="" style="width:">AcdEF</button>
                <button class="u20px frame swing" judul="tombol ini radius 20px" onclick="" style="width:">BcDefG</button>
                <button class="u10px" onclick="" style="width:">Cdefg</button>
                <button class="r8px" onclick="" style="width:">DefGh</button>
                <button class="u1px" onclick="" style="width:">EfGhij</button>

            </section>
   <br />
            <section class="grup-tmb-v" style="width:auto">
                <p>
                    grup vertikal : animasi latar berubah
                </p>
                <button class="frame fade" judul="ukuran 50%" onclick="" style="width:50%">Abcde</button>
                <button onclick="" style="width:50%">BcDefg</button>
                <button class="frame aframe" onclick="" style="width:50%">CdEfgh
                    <span class="teks">tombol ini ukuran 50%</span></button>
                <button onclick="" style="width:90%">DefGHi</button>
                <button onclick="" style="width:40%">EFgHI</button>
                <button onclick="" style="width:15%">F</button>
                <button onclick="" style="width:60%">G</button>
                <br />
            </section>
```
## Membangun Tabel
### tabel default 
```html
<table class="tabel ta l80">
                <tr>
                    <th>Nama</th>
                    <th>Class</th>
                </tr>
                <tr>
                    <td>Hijau</td>
                    <td>hijau</td>
                </tr>
            </table>
```
### tabel modifikasi
```html
  <input type="text" id="ketikkan" onkeyup="fungsicariTabel()" placeholder="cari nama..">
            <table id="caritabel" class="tabel-magenta">
                <tr>
                    <th>Nama</th>
                    <th>Class</th>
                </tr>
                <tr>
                    <td>Hijau</td>
                    <td>hijau</td>
                </tr>
                <tr>
                    <td>Merah</td>
                    <td>merah</td>
                </tr>
                <tr>
                    <td>Magenta</td>
                    <td>magenta</td>
                </tr>
            </table>
```
# [Lanjutkan Dokumentasi atau Tutorial](https://github.com/nelsenpro/frame/blob/main/framecss/2.1.23.Alpha/dokumentasi.md)

## Creators
[*Nelsen Niko*](https://wa.me/6285328736706/)
<!-- Text -->

## Thanks
[Normalize.css](https://necolas.github.io/normalize.css/) | [Animate.css](https://animate.style/) | [Fontsawesome](https://fontawesome.com/) | 





 
