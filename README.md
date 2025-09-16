# Saya akan menjelaskan file Portofolio.html, gallery.html, tentang.html, dan style.css 
## 1. Portofolio.html
```html
<!DOCTYPE html> <!-- Menentukan bahwa dokumen ini adalah HTML5 -->
<html lang="id"> <!-- Awal dokumen HTML, dengan bahasa Indonesia -->
<head>  
  <meta charset="UTF-8"> <!-- Mengatur karakter encoding menjadi UTF-8 -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Supaya responsif di perangkat mobile -->
  <title>Portofolio</title> <!-- Judul halaman yang tampil di tab browser -->
  <link rel="stylesheet" href="style.css"> <!-- Menghubungkan file CSS eksternal -->
</head>  

<body>  
  <div class="nav-container" id="nav"> <!-- Kontainer navigasi utama -->

    <div class="menu left"><a href="tentang.html">Tentang Saya</a></div> <!-- Menu sebelah kiri, link ke tentang.html -->

    <div class="profile" id="profile"> <!-- Foto profil di tengah -->
      <img src="gambar1.png" alt="Foto Profil"> <!-- Gambar profil -->
    </div>

    <div class="menu right"><a href="gallery.html">Gallery</a></div> <!-- Menu sebelah kanan, link ke gallery.html -->

  </div>

  <script>
    const profile = document.getElementById('profile'); // Mengambil elemen dengan id="profile"
    const nav = document.getElementById('nav'); // Mengambil elemen dengan id="nav"

    profile.addEventListener('click', () => { // Memberi event ketika profil diklik
      nav.classList.toggle('active'); // Menambahkan/menghapus class "active" agar menu muncul
    });
  </script>
</body>  
</html>

```
## 2. style.css
```html
body {
  margin: 0; /* Menghapus margin bawaan browser */
  height: 100vh; /* Tinggi halaman = 100% layar */
  display: flex; /* Menggunakan flexbox untuk tata letak */
  justify-content: center; /* Elemen dipusatkan secara horizontal */
  align-items: center; /* Elemen dipusatkan secara vertikal */
  background: #1e1e1e; /* Warna latar hitam keabu-abuan */
  font-family: Arial, sans-serif; /* Font utama Arial */
}

.nav-container {
  position: relative; /* Posisi relatif agar menu bisa ditempatkan absolut */
  display: flex; /* Susun isi secara horizontal */
  align-items: center; /* Elemen rata tengah secara vertikal */
}

.profile {
  width: 120px; /* Lebar foto profil */
  height: 120px; /* Tinggi foto profil */
  border-radius: 50%; /* Membuat bentuk lingkaran */
  border: 3px solid white; /* Garis tepi putih */
  cursor: pointer; /* Ubah kursor jadi tangan saat diarahkan */
  z-index: 2; /* Supaya selalu di atas elemen lain */
  overflow: hidden; /* Potong gambar biar ikut bulat */
  justify-content: center; /* Konten di tengah */
  align-items: center;
  background: #333; /* Warna latar abu gelap */
  transition: transform 0.3s ease; /* Animasi halus saat hover */
}

.profile:hover {
  transform: scale(1.05); /* Perbesar sedikit saat kursor diarahkan */
}

.profile img {
  width: 100%; /* Gambar memenuhi wadah */
  height: 100%; 
  object-fit: cover; /* Gambar menyesuaikan tanpa merusak rasio */
  border-radius: 50%; /* Pastikan tetap bulat */
}

.menu {
  position: absolute; /* Posisi mutlak, relatif ke nav-container */
  top: 50%; /* Posisi di tengah vertikal */
  transform: translateY(-50%); /* Koreksi agar benar-benar di tengah */
  background: #333; /* Warna latar menu */
  color: white; /* Warna teks putih */
  padding: 15px 25px; /* Ruang dalam menu */
  border-radius: 8px; /* Membulatkan sudut */
  opacity: 0; /* Awalnya transparan (tidak terlihat) */
  pointer-events: none; /* Tidak bisa diklik jika belum aktif */
  transition: all 0.3s ease; /* Animasi saat muncul */
  font-weight: bold; /* Teks tebal */
}

.menu.left {
  left: -180px; /* Menu kiri bergeser keluar layar */
}

.menu.right {
  right: -180px; /* Menu kanan bergeser keluar layar */
}

.nav-container.active .menu {
  opacity: 1; /* Jadi terlihat */
  pointer-events: auto; /* Bisa diklik */
}

.menu:hover {
  background: #444; /* Warna lebih terang saat hover */
}

.menu a {
  color: white; /* Warna teks link putih */
  text-decoration: none; /* Hilangkan garis bawah */
}

```
## 3. tentang.html
```html
<!DOCTYPE html> <!-- Dokumen HTML5 -->
<html lang="id"> <!-- Bahasa Indonesia -->
<head>
  <meta charset="UTF-8"> <!-- Encoding UTF-8 -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Responsif di mobile -->
  <title>Tentang Saya</title> <!-- Judul tab -->
  <style>
    body {
      font-family: Arial, sans-serif; /* Font utama */
      background: #000; /* Latar belakang hitam */
      color: #fff; /* Teks putih */
      padding: 40px; /* Jarak isi halaman */
      display: flex;
      flex-direction: column; /* Susun konten secara kolom */
      align-items: center; /* Konten di tengah */
    }

    .container {
      display: flex; /* Susun horizontal */
      gap: 40px; /* Jarak antar elemen */
      margin-top: 30px;
      align-items: flex-start; /* Rata atas */
    }

    .kiri {
      display: flex;
      flex-direction: column; /* Susun ke bawah */
      gap: 20px; /* Jarak antar elemen */
    }

    .foto img {
      width: 250px; /* Lebar foto */
      height: auto; /* Tinggi menyesuaikan */
      border-radius: 10px; /* Sudut melengkung */
    }

    .hobi {
      background: rgba(255,255,255,0.1); /* Kotak transparan */
      padding: 15px;
      border-radius: 10px;
    }

    .biografi {
      max-width: 400px; /* Batas lebar */
      background: rgba(255,255,255,0.1);
      padding: 20px;
      border-radius: 10px;
    }

    a {
      color: #00bcd4; /* Warna link biru muda */
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline; /* Garis bawah saat hover */
    }
  </style>
</head>
<body>
  <h1>Tentang Saya</h1> <!-- Judul utama -->
  <p>Halo, saya Darmawansyahmurfa</p> <!-- Perkenalan singkat -->

  <div class="container"> <!-- Pembungkus kiri (foto+hobi) dan kanan (biografi) -->
    <div class="kiri">
      <div class="foto">
        <img src="saya.jpg" alt="Foto Saya"> <!-- Foto -->
      </div>
      <div class="hobi">
        <h3>Hobi Saya</h3> <!-- Judul hobi -->
        <p>Main catur</p>
        <p>Bersepeda</p>
        <p>Baca komik</p>
      </div>
    </div>

    <div class="biografi"> <!-- Bagian biografi -->
      <h3>Biografi</h3>
      <p>Nama saya Darmawansyah Murfa, berumur 19 tahun, Saya seorang adalah seorang mahasiswa yang tertarik dengan dunia teknologi, pemrograman, dan desain web. Halaman ini saya buat untuk memperkenalkan diri.</p>
    </div>
  </div>

  <p style="margin-top: 20px;">
    <a href="portopolio.html">Kembali ke Halaman Utama</a> <!-- Link balik -->
  </p>
</body>
</html>

```

## 4. gallery.html
```html
<!DOCTYPE html> <!-- Dokumen HTML5 -->
<html lang="id">
<head>
  <meta charset="UTF-8"> <!-- Encoding UTF-8 -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Responsif -->
  <title>Gallery</title> <!-- Judul tab -->
  <style>
    body {
      font-family: Arial, sans-serif; /* Font utama */
      background: #181818; /* Latar belakang abu gelap */
      padding: 40px; /* Jarak isi */
    }
    .gallery {
      display: grid; /* Tampilkan dalam bentuk grid */
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); /* Otomatis menyesuaikan ukuran layar */
      gap: 15px; /* Jarak antar gambar */
    }
    .gallery img {
      width: 100%; /* Gambar memenuhi kolom */
      border-radius: 8px; /* Sudut melengkung */
    }
  </style>
</head>
<body>
  <h1 style="color: #ffffff;">Gallery</h1> <!-- Judul halaman -->
  <div class="gallery">
    <img src="gambar2.jpg" alt="Foto 1"> <!-- Gambar pertama -->
    <img src="gambar3.jpg" alt="Foto 2"> <!-- Gambar kedua -->
    <img src="gambar4.jpg" alt="Foto 3"> <!-- Gambar ketiga -->
  </div>
  <br>
  <a href="portopolio.html">Kembali ke Halaman Utama</a> <!-- Link balik -->
</body>
</html>


```
