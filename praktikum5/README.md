# Praktikum 5

Berikut adalah analsisinya

## 2a [`praktikum5/2a.HTML`](praktikum5/2a.HTML)
Output: 

![gambar1tagScript.png](praktikum5/2a.png)

Analisis:
- Pada tag <script> terdapat atribut language="JavaScript" yang menandakan bahwa script menggunakan bahasa pemrograman JavaScript.
- Di dalam tag <head> terdapat script dengan perintah document.write("Program JavaScript Aku di kepala") yang berfungsi menampilkan teks “Program JavaScript Aku di kepala”.
- Di dalam tag <body> terdapat script dengan perintah document.write("Program JavaScript Aku di body") yang berfungsi menampilkan teks “Program JavaScript Aku di body”.

## 2.c [`praktikum5/2c.html`](praktikum5/2c.html)
Output:
  
  ![praktikum5/2c.png](praktikum5/2c.png)

Analisis :
- Pada tag <button> terdapat atribut onclick="tampilkan_nama()" yang berarti ketika tombol diklik, maka fungsi JavaScript tampilkan_nama() akan dijalankan.
- Pada tag <div id="hasil"></div> dibuat sebuah elemen kosong dengan id hasil, yang nantinya akan diisi teks dari fungsi JavaScript.
- Di dalam tag <script> dibuat sebuah fungsi tampilkan_nama(). Fungsi ini menggunakan document.getElementById("hasil").innerHTML untuk menampilkan teks "Nama Saya Adalah Andi Akram Nur Risal" ke dalam elemen <div> dengan id hasil.

## 2.d [`praktikum5/3.html`](praktikum5/3.html)
Output:

![praktikum5/2d.png](praktikum5/2d.png)

Analisis:
- Pada tag <script language="JavaScript"> dituliskan kode JavaScript. Atribut language="JavaScript" menandakan bahwa script menggunakan bahasa JavaScript (meskipun di HTML5 atribut ini sudah tidak digunakan lagi).

- Di dalam script terdapat perintah var nama = prompt("Siapa nama Anda?"); yang berfungsi menampilkan kotak dialog input (prompt) kepada pengguna untuk mengetikkan nama. Nilai yang dimasukkan akan disimpan ke dalam variabel nama.

- Perintah document.write("Hai, " + nama); digunakan untuk menuliskan teks ke halaman. Teks yang ditampilkan adalah "Hai, [nama]" sesuai dengan input yang dimasukkan user.
## 4. [`praktikum5/4.html`](praktikum5/4.html)
Output:
  
  ![praktikum5/4.png](praktikum5/4.png)
Analisis:
- Pada tag <script language="JavaScript"> dituliskan kode JavaScript yang akan dijalankan ketika halaman dimuat.

- Perintah window.alert("apakah anda akan meninggalkan halaman ini") berfungsi menampilkan kotak dialog alert berisi pesan teks "apakah anda akan meninggalkan halaman ini".

- window.alert() bisa juga ditulis cukup dengan alert(), karena alert sudah otomatis merujuk ke objek window di JavaScript.

## 4.2 [`praktikum5/4,2.html`](praktikum5/4,2.html)
Output:
![praktikum5/4,2.png](praktikum5/4,2.png)

Analisis:
- Pada tag <script language="JavaScript"> dituliskan kode JavaScript. Atribut language="JavaScript" menandakan bahwa script menggunakan bahasa JavaScript (meskipun di HTML5 atribut ini sudah tidak digunakan lagi).

- Perintah var jawaban = window.confirm("Apakah anda sudah yakin ?"); menampilkan kotak dialog konfirmasi (confirm box) kepada pengguna dengan tombol OK dan Cancel. Nilai yang dipilih pengguna akan disimpan di variabel jawaban (true jika OK, false jika Cancel).

## 5.a [`praktikum5/5a.html`](praktikum5/5a.html)
Output:
  
  ![praktikum5/5a.png](praktikum5/5a.png)

Analisis:
- Tag <script language="JavaScript"> menandakan bahwa kode di dalamnya menggunakan bahasa JavaScript (atribut language sudah usang, di HTML5 bisa dihilangkan).
- var VariabelKu; → mendeklarasikan sebuah variabel kosong bernama VariabelKu.
- var VariabelKu2 = 3; → mendeklarasikan variabel VariabelKu2 dan langsung memberi nilai 3.
- VariabelKu = 1234; → memberi nilai 1234 ke variabel VariabelKu.
- document.write(VariabelKu*VariabelKu2); → menghitung hasil perka

## 5.b [`praktikum5/5b.html`](praktikum5/5b.html)
Output:

![praktikum5/5b.png](praktikum5/5b.png)

Analisis:
- Tag <script> digunakan untuk menulis kode JavaScript di dalam dokumen HTML.
- var a = 12; dan var b = 4; → mendeklarasikan dua variabel, a dengan nilai awal 12 dan b dengan nilai 4.
- function Perkalian_Dengan2(b) → mendefinisikan fungsi bernama Perkalian_Dengan2 yang menerima satu parameter b.
   - Di dalam fungsi, perintah a = b * 2; menghitung dua kali nilai b dan menyimpan hasilnya ke variabel a.
   - return a; mengembalikan nilai hasil perkalian.
- document.write("Dua kali dari " + b + " adalah " + Perkalian_Dengan2(b) + "<br>");
   - Memanggil fungsi Perkalian_Dengan2(b) dengan b = 4.
   - Fungsi mengembalikan 4 * 2 = 8 dan hasilnya ditulis ke halaman:
     ```html
     Dua kali dari 4 adalah 8
     ```
- document.write("Nilai dari a adalah " + a);
   - Menuliskan nilai terbaru dari variabel a setelah diproses fungsi, yaitu 8.
   - Hasilnya di halaman:
     ```html
     Nilai dari a adalah 8
     ```

## 5.b2 [`praktikum5/5b2.html`](praktikum5/5b2.html)
Output:

![praktikum5/5b2.png](praktikum5/5b2.png)

Analisis:
- Tag <script language="JavaScript"> digunakan untuk menulis kode JavaScript. Atribut language sudah usang, tapi di sini menandakan bahwa script menggunakan JavaScript.
- var a = 12; dan var b = 4; → mendeklarasikan dua variabel global, a dengan nilai 12 dan b dengan nilai 4.
- Fungsi PerkalianDengan2(b) → mendefinisikan fungsi yang menerima parameter b.
   - Di dalam fungsi, var a = b * 2; mendeklarasikan variabel lokal a yang nilainya adalah dua kali b.
   - return a; mengembalikan nilai hasil perkalian tersebut.
- document.write("dua kali dari",b,"adalah", PerkalianDengan2b(b)) → di sini ada kesalahan

## 7. [`praktikum5/7.html`](praktikum5/7.html)
Output:

![praktikum5/7.png](praktikum5/7.png)

Analisis:
- parseInt() mengubah nilai menjadi bilangan bulat. Contohnya: parseInt(27) → 27, parseInt(27.5) → 27, parseInt("27A") → 27, parseInt("A27.5") → NaN.
- parseFloat() mengubah nilai menjadi bilangan desimal. Contohnya: parseFloat(27) → 27, parseFloat(27.5) → 27.5, parseFloat("27A") → 27, parseFloat("A27.5") → NaN.
- document.write() menampilkan hasil konversi ke halaman web.

## 8. [`praktikum5/8.html`](praktikum5/8.html)
Output:

![gambar10konversiTipeData.png](ImageOutput/gambar10konversiTipeData.png)

Analisis:
- Tag <script language="JavaScript"> menandakan bahwa kode di dalamnya menggunakan JavaScript (atribut language sudah usang di HTML5).
- Perintah document.write() digunakan untuk menampilkan hasil operasi matematika langsung ke halaman web.
- Operasi yang dilakukan:
   - 2 + 3 → menjumlahkan dua angka → hasil 5.
   - 20 - 3 → mengurangi angka → hasil 17.
   - 2 * 3 → perkalian → hasil 6. (Catatan: ada typo di kode, tulisan "20* 3" tetapi operasi tetap 2 * 3)
   - 40 / 3 → pembagian → hasil 13.333333333333334 (JavaScript menampilkan desimal panjang).
- "<BR>" digunakan untuk membuat baris baru di halaman sehingga hasil setiap operasi muncul di baris terpisah.

## 9. [`praktikum5/9.html`](praktikum5/9.html)
Output:

![praktikum5/9.png](Ipraktikum5/9.png)

Analisis:
- Tag <script language="JavaScript"> menandakan bahwa kode di dalamnya menggunakan JavaScript (atribut language sudah usang di HTML5).
- var nilai = prompt("Nilai (0-100): ", 0);
   - Menampilkan kotak dialog input (prompt) untuk memasukkan nilai antara 0–100.
   - Nilai yang dimasukkan user disimpan di variabel nilai.
- var hasil = (nilai >= 60) ? "Lulus" : "Tidak Lulus";
   - Menggunakan operator ternary (? :).
   - Artinya: jika nilai >= 60, maka hasil berisi "Lulus"; jika kurang dari 60, hasil berisi "Tidak Lulus".
- document.write("Hasil: " + hasil);
   - Menampilkan hasil ke halaman web.

## tugas 1  [`praktikum5/TugasMandiri1.html`](praktikum5/TugasMandiri1.html)
Output:

  ![praktikum5/tugasmandiri1.png](praktikum5/tugasmandiri1.png)


## Tugas 2 [`praktikum5/TugasMandiri2.html`](praktikum5/TugasMandiri2.html)
Output:

![praktikum5/tugasmandiri2.png](praktikum5/tugasmandiri2.png)

## Tugas 3 [`praktikum5/TugasMandiri3.html`](praktikum5/TugasMandiri3.html)
Output:
- Gambar Input 1

![praktikum5/tugasmandiri3.png](praktikum5/tugasmandiri3.png)


## Tugas 4 [`praktikum5/TugasMandiri4.html`](praktikum5/TugasMandiri4.html)
Output:

![praktikum5/tugasmandiri4.png](praktikum5/tugasmandiri4.png)
