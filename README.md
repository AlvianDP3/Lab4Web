# Langkah-langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut.

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Box Element</title>
</head>
<body>
  <header>
      <h1>Box Element</h1>
  </header>
</body>
</html>
```

# Membuat Box Element
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut.
```
<section>
  <div class="div1">Div 1</div>
  <div class="div2">Div 2</div>
  <div class="div3">Div 3</div>
</section>
```
# CSS Float Property
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut.
```
<style>
  div {
      float:left;
      padding: 10px;
}
.div1 {
  background: red;
}
.div2 {
  background: yellow;
}
.div3 {
  background: green;
}
</style>
```
Kemudian buka browser untuk melihat hasilnya.

![Membuat Box Element dan CSS Float Property](https://user-images.githubusercontent.com/56244029/115818653-6cbdf400-a427-11eb-9b6e-5acb56f38910.png)

# Mengatur Clearfix Element
Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk
mengaturnya.
Tambahkan element div lainnya seteleah div3 seperti berikut.
```
<section>
  <div class="div1">Div 1</div>
  <div class="div2">Div 2</div>
  <div class="div3">Div 3</div>
  <div class="div4">Div 4</div>
</section>
```
Kemudian atur property clear pada CSS, seperti berikut.
```
.div4 {
  background-color: blue;
  clear: left;
  float: none;
}
```
Selanjutnya buka browser dan refresh kembali.

![Mengatur Clearfix Element](https://user-images.githubusercontent.com/56244029/115818767-a7c02780-a427-11eb-85b6-daa33552cd49.png)

# Membuat Layout Sederhana
Kita akan membuat layout web sederhana seperti gambar berikut.

![1](https://user-images.githubusercontent.com/56244029/115818848-d9d18980-a427-11eb-961f-d98fdd7efee4.jpg)

Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama
home.html, dan file css dengan nama style.css.
```
<!DOCTYPE html>
  <html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
    
    </div>
</body>
</html>

Kemudian buat kerangka layout dengan semantics element seperti berikut.

![2](https://user-images.githubusercontent.com/56244029/115818998-303ec800-a428-11eb-9996-a4b0b8e5a4a6.jpg)

Kemudian tulis kode berikut.

```
<header>
<h1>Layout Sederhana</h1>
</header>
<nav>
<a href="home.html" class="active">Home</a>
<a href="artikel.html">Artikel</a>
<a href="about.html">About</a>
<a href="kontak.html">Kontak</a>
</nav>
<section id="hero"></section>
<section id="wrapper">
<section id="main"></section>
<aside id="sidebar"></aside>
</section>
<footer>
<p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```

![Membuat Navigasi layeout](https://user-images.githubusercontent.com/56244029/115819201-90ce0500-a428-11eb-9350-598a52f9e88c.png)

Kemudian tambahkan kode CSS untuk membuat layoutnya.

```
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400
;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0
,300;0,700;1,300&display=swap');
/* Reset CSS */
* {
margin: 0;
padding: 0;
}
body {
line-height:1;
font-size:100%;
font-family:'Open Sans', sans-serif;
color:#5a5a5a;
}
#container {
width: 980px;
margin: 0 auto;
box-shadow: 0 0 1em #cccccc;
}
/* header */
header {
padding: 20px;
}
header h1 {
margin: 20px 10px;
color: #b5b5b5;
}


Kemudian lihat hasilnya pada browser.

![Membuat Layout Sederhana](https://user-images.githubusercontent.com/56244029/115819264-b0fdc400-a428-11eb-953e-01bac447192a.png)

# Membuat Navigasi
Kemudian selanjutnya mengatur navigasi.

```
/* navigasi */
nav {
display: block;
background-color: #1f5faa;
}
nav a {
padding: 15px 30px;
display: inline-block;
color: #ffffff;
font-size: 14px;
text-decoration: none;
font-weight: bold;
}
nav a.active,
nav a:hover {
background-color: #2b83ea;
}
```
Kemudian lihat hasilnya.

![Membuat Navigasi](https://user-images.githubusercontent.com/56244029/115819524-32555680-a429-11eb-86fa-45ba70b78288.png)

# Membuat Hero Panel.
Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.
```
HTML
<section id="hero">
<h1>Hello World!</h1>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
<a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```
/* Hero Panel */
#hero {
background-color: #e4e4e5;
padding: 50px 20px;
margin-bottom: 20px;
}
#hero h1 {
margin-bottom: 20px;
font-size: 35px;
}
#hero p {
margin-bottom: 20px;
font-size: 18px;
line-height:

![Membuat Hero Panel](https://user-images.githubusercontent.com/56244029/115819630-6c265d00-a429-11eb-8c3a-20942fe5cc00.png)


