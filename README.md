# 💡 Penjelasan CSS 💡
CSS (Cascading Style Sheets) adalah bahasa stylesheet yang digunakan untuk mengatur tampilan, tata letak, warna, dan font elemen HTML pada situs web. CSS memisahkan konten (HTML) dari visualisasi, membuat website lebih menarik, responsif, dan mudah dikelola. Tanpa CSS, halaman web hanya berupa **teks polos berstruktur.**. 

---

## Cara menghubungkan CSS ada 3 yaitu:

- **Inline CSS**  
  Menyisipkan style di setiap tag HTML.  
  ```html
  <p style="color: red; font-size: 18px;">
    Teks ini menggunakan Inline CSS
  </p>

- **Internal CSS**  
  Membuat file CSS dengan tag `<style>` pada bagian `<head>`.  
  ```html
  <head>
    <style>
      p {
        color: blue;
        font-size: 20px;
      }
    </style>
  </head>
  <body>
    <p>Teks ini menggunakan Internal CSS</p>
  </body>

- **External CSS**  
  Membuat file CSS terpisah dan menghubungkannya dengan `<link>`.  
  ```html
  <head>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <p>Teks ini menggunakan External CSS</p>
  </body>

# 💫 Property dan Value dasar CSS 💫

## 📌 Color Styling 📌

- **Color**📎  
  Untuk memberikan warna pada elemen HTML.  
  Value `color` ada 3 yaitu:  

  1. **Nama warna**  
     ```html
     <p style="color: red;">Teks warna merah</p>
     ```

  2. **RGB**  
     ```html
     <p style="color: rgb(0, 128, 0);">Teks warna hijau</p>
     ```

  3. **Hexadecimal**  
     ```html
     <p style="color: #0000FF;">Teks warna biru</p>
     ```

## 📌 Background Styling 📌

- **Background-Color**📎  
  Untuk memberikan warna latar belakang pada elemen HTML.  
  Dengan ini, kamu bisa mengatur warna area di belakang teks, gambar, atau konten lain dalam sebuah elemen.  
  Value `background-color` ada 4 yaitu:  

  1. **Color (nama warna)**  
     ```html
     <div style="background-color: yellow;">
       Latar belakang kuning
     </div>
     ```

  2. **RGB**  
     ```html
     <div style="background-color: rgb(0, 128, 128);">
       Latar belakang hijau kebiruan
     </div>
     ```

  3. **Hexadecimal**  
     ```html
     <div style="background-color: #FF5733;">
       Latar belakang oranye
     </div>
     ```

  4. **Inherit**  
     ```html
     <div style="background-color: inherit;">
       Latar belakang mengikuti elemen induk
     </div>
     ```
     
- **Background-Image**📎  
  Untuk memberikan gambar latar belakang pada sebuah elemen HTML.  
  Value `background-image` ada 1 yaitu: `url()`.  

  ```html
  <div style="background-image: url('sample.jpg');">
    Konten dengan gambar latar belakang
  </div>

- **Background-Position**📎  
  Untuk mengatur posisi gambar latar belakang dalam sebuah elemen.  
  Dengan ini, kamu bisa menentukan apakah gambar berada di kiri, kanan, tengah, atas, bawah, atau posisi khusus menggunakan nilai koordinat.  
  Value `background-position` ada 7 yaitu:  

  1. **Top**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: top;">
       Latar belakang di atas
     </div>
     ```

  2. **Bottom**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: bottom;">
       Latar belakang di bawah
     </div>
     ```

  3. **Left**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: left;">
       Latar belakang di kiri
     </div>
     ```

  4. **Right**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: right;">
       Latar belakang di kanan
     </div>
     ```

  5. **Px (pixel)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: 50px 100px;">
       Latar belakang dengan koordinat pixel
     </div>
     ```

  6. **% (persentase)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: 50% 50%;">
       Latar belakang di tengah (persentase)
     </div>
     ```

  7. **em (relative unit)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: 2em 3em;">
       Latar belakang dengan posisi relatif em
     </div>
     ```
     
- **Background-Repeat**📎  
  Untuk mengatur apakah gambar latar belakang (`background-image`) diulang atau tidak, serta bagaimana pola pengulangannya ditampilkan dalam sebuah elemen.  
  Value `background-repeat` ada 6 yaitu:  

  1. **No-repeat**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: no-repeat;">
       Latar belakang tidak diulang
     </div>
     ```

  2. **repeat-x**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: repeat-x;">
       Latar belakang diulang secara horizontal
     </div>
     ```

  3. **repeat-y**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: repeat-y;">
       Latar belakang diulang secara vertikal
     </div>
     ```

  4. **space**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: space;">
       Latar belakang diulang dengan jarak antar gambar
     </div>
     ```

  5. **round**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: round;">
       Latar belakang diulang dan disesuaikan ukurannya
     </div>
     ```

  6. **space repeat**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: space repeat;">
       Kombinasi pengulangan dengan jarak dan pola
     </div>
     ```
     
- **Background-Size**📎  
  Untuk mengatur ukuran gambar latar belakang pada sebuah elemen.  
  Dengan ini, kamu bisa menentukan apakah gambar memenuhi seluruh area, menyesuaikan proporsi, atau menggunakan ukuran khusus.  
  Value `background-size` ada 4 yaitu:  

  1. **Cover**  
     ```html
     <div style="background-image: url('sample.jpg'); background-size: cover;">
       Latar belakang memenuhi seluruh area
     </div>
     ```

  2. **Contain**  
     ```html
     <div style="background-image: url('sample.jpg'); background-size: contain;">
       Latar belakang menyesuaikan proporsi
     </div>
     ```

  3. **Px (pixel)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-size: 200px 100px;">
       Latar belakang dengan ukuran khusus pixel
     </div>
     ```

  4. **% (persentase)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-size: 50% 50%;">
       Latar belakang dengan ukuran persentase
     </div>
     ```

## 📌 Font-Styling 📌

- **Font-Family**📎  
  Untuk menentukan jenis huruf (font) yang dipakai pada teks dalam elemen HTML.  
  Dengan ini, kamu bisa mengatur tipografi agar sesuai dengan branding, estetika, atau keterbacaan.  
  Value `font-family` ditentukan oleh jenis font yang digunakan.  

  Contoh penggunaan:  
  ```html
  <p style="font-family: Arial, sans-serif;">
    Teks dengan font Arial
  </p>

- **Font-Size**📎  
  Untuk mengatur ukuran teks dalam elemen HTML.  
  Dengan ini, kamu bisa membuat teks lebih besar, lebih kecil, atau responsif sesuai kebutuhan desain.  
  Value `font-size` ada 8 yaitu:  

  1. **Rem**  
     ```html
     <p style="font-size: 1rem;">Teks ukuran 1rem</p>
     ```

  2. **Em**  
     ```html
     <p style="font-size: 1.5em;">Teks ukuran 1.5em</p>
     ```

  3. **Px (pixel)**  
     ```html
     <p style="font-size: 20px;">Teks ukuran 20px</p>
     ```

  4. **Vw (viewport width)**  
     ```html
     <p style="font-size: 5vw;">Teks ukuran 5vw</p>
     ```

  5. **Vh (viewport height)**  
     ```html
     <p style="font-size: 5vh;">Teks ukuran 5vh</p>
     ```

  6. **% (persentase)**  
     ```html
     <p style="font-size: 120%;">Teks ukuran 120%</p>
     ```

  7. **Small**  
     ```html
     <p style="font-size: small;">Teks ukuran kecil</p>
     ```

  8. **Large**  
     ```html
     <p style="font-size: large;">Teks ukuran besar</p>
     ```

- **Font-Weight**📎  
  Untuk mengatur ketebalan huruf (tebal-tipis) pada teks.  
  Dengan ini, kamu bisa membuat teks tampil normal, lebih tipis, atau lebih tebal sesuai kebutuhan tipografi.  
  Value `font-weight` ada 5 yaitu:  

  1. **normal**  
     ```html
     <p style="font-weight: normal;">Teks normal</p>
     ```

  2. **lighter**  
     ```html
     <p style="font-weight: lighter;">Teks lebih tipis</p>
     ```

  3. **bold**  
     ```html
     <p style="font-weight: bold;">Teks tebal</p>
     ```

  4. **bolder**  
     ```html
     <p style="font-weight: bolder;">Teks lebih tebal</p>
     ```

  5. **100–900 (angka)**  
     ```html
     <p style="font-weight: 100;">Teks sangat tipis</p>
     <p style="font-weight: 400;">Teks normal</p>
     <p style="font-weight: 700;">Teks tebal</p>
     <p style="font-weight: 900;">Teks super tebal</p>
     ```
     
- **Font-Variant**📎  
  Untuk mengatur variasi gaya font, terutama dalam hal *small-caps* (huruf kecil ditampilkan sebagai huruf kapital kecil).  
  Dengan ini, teks bisa tampil lebih formal atau bergaya tipografi khusus tanpa mengubah isi asli teks.  
  Value `font-variant` ada 3 yaitu:  

  1. **normal**  
     ```html
     <p style="font-variant: normal;">Teks normal</p>
     ```

  2. **small-caps**  
     ```html
     <p style="font-variant: small-caps;">Teks dengan small-caps</p>
     ```

  3. **inherit**  
     ```html
     <p style="font-variant: inherit;">Teks mengikuti font-variant dari elemen induk</p>
     ```
     
- **Font-Style**📎  
  Untuk mengatur gaya huruf miring atau normal pada teks.  
  Dengan ini, kamu bisa menampilkan teks dalam bentuk *italic*, *oblique*, atau tetap normal sesuai kebutuhan tipografi.  
  Value `font-style` ada 4 yaitu:  

  1. **normal**  
     ```html
     <p style="font-style: normal;">Teks normal</p>
     ```

  2. **italic**  
     ```html
     <p style="font-style: italic;">Teks miring (italic)</p>
     ```

  3. **oblique**  
     ```html
     <p style="font-style: oblique;">Teks miring (oblique)</p>
     ```

  4. **inherit**  
     ```html
     <p style="font-style: inherit;">Teks mengikuti font-style dari elemen induk</p>
     ```
     
- **Line-Height**📎  
  Untuk mengatur tinggi baris teks dalam sebuah elemen.  
  Dengan kata lain, ia menentukan jarak vertikal antara garis dasar (baseline) teks satu dengan teks berikutnya.  
  Value `line-height` ada 4 yaitu:  

  1. **normal**  
     ```html
     <p style="line-height: normal;">Teks dengan line-height normal</p>
     ```

  2. **em**  
     ```html
     <p style="line-height: 2em;">Teks dengan line-height 2em</p>
     ```

  3. **px (pixel)**  
     ```html
     <p style="line-height: 30px;">Teks dengan line-height 30px</p>
     ```

  4. **% (persentase)**  
     ```html
     <p style="line-height: 150%;">Teks dengan line-height 150%</p>
     ```
## 📌 Text Styling 📌

- **Text-Align**📎  
  Untuk mengatur perataan teks secara horizontal di dalam sebuah elemen blok.  
  Value `text-align` ada 4 yaitu:  

  1. **start**  
     ```html
     <p style="text-align: start;">Teks rata kiri (default)</p>
     ```

  2. **end**  
     ```html
     <p style="text-align: end;">Teks rata kanan</p>
     ```

  3. **center**  
     ```html
     <p style="text-align: center;">Teks rata tengah</p>
     ```

  4. **justify**  
     ```html
     <p style="text-align: justify;">
       Teks rata kiri dan kanan, membuat tampilan lebih rapi seperti paragraf koran
     </p>
     ```
     
- **Text-Indent**📎  
  Untuk memberikan indentasi (jarak masuk) pada baris pertama teks dalam sebuah elemen blok, misalnya paragraf `<p>`.  
  Value `text-indent` ada 4 yaitu:  

  1. **px (pixel)**  
     ```html
     <p style="text-indent: 40px;">
       Paragraf dengan indentasi 40px
     </p>
     ```

  2. **% (persentase)**  
     ```html
     <p style="text-indent: 10%;">
       Paragraf dengan indentasi 10% dari lebar elemen
     </p>
     ```

  3. **em (relative unit)**  
     ```html
     <p style="text-indent: 2em;">
       Paragraf dengan indentasi 2em
     </p>
     ```

  4. **inherit**  
     ```html
     <p style="text-indent: inherit;">
       Paragraf mengikuti indentasi dari elemen induk
     </p>
     ```

- **Text-Decoration**📎  
  Untuk memberikan efek dekorasi pada teks, seperti garis bawah, garis atas, coretan, atau menghilangkan dekorasi bawaan (misalnya pada link).  
  Value `text-decoration` ada 4 yaitu:  

  1. **none**  
     ```html
     <p style="text-decoration: none;">Teks tanpa dekorasi</p>
     ```

  2. **underline**  
     ```html
     <p style="text-decoration: underline;">Teks dengan garis bawah</p>
     ```

  3. **overline**  
     ```html
     <p style="text-decoration: overline;">Teks dengan garis atas</p>
     ```

  4. **line-through**  
     ```html
     <p style="text-decoration: line-through;">Teks dengan coretan</p>
     ```
     
- **Text-Transform**📎  
  Untuk mengubah tampilan huruf pada teks tanpa mengubah isi asli di HTML.  
  Jadi, teks tetap sama di kode, tetapi tampilannya bisa diubah menjadi huruf besar, kecil, atau kapitalisasi awal kata.  
  Value `text-transform` ada 4 yaitu:  

  1. **uppercase**  
     ```html
     <p style="text-transform: uppercase;">Teks menjadi huruf BESAR</p>
     ```

  2. **lowercase**  
     ```html
     <p style="text-transform: lowercase;">Teks menjadi huruf kecil</p>
     ```

  3. **capitalize**  
     ```html
     <p style="text-transform: capitalize;">Teks Kapitalisasi Awal Kata</p>
     ```

  4. **inherit**  
     ```html
     <p style="text-transform: inherit;">Teks mengikuti text-transform dari elemen induk</p>
     ```
     
- **Letter-Spacing**📎  
  Untuk mengatur jarak antar huruf (spasi horizontal) dalam teks.  
  Dengan ini, kamu bisa membuat teks terlihat lebih renggang, rapat, atau memiliki efek tipografi tertentu.  
  Value `letter-spacing` ada 3 yaitu:  

  1. **normal**  
     ```html
     <p style="letter-spacing: normal;">Teks dengan jarak huruf normal</p>
     ```

  2. **px (pixel)**  
     ```html
     <p style="letter-spacing: 5px;">Teks dengan jarak huruf 5px</p>
     ```

  3. **em (relative unit)**  
     ```html
     <p style="letter-spacing: 0.2em;">Teks dengan jarak huruf 0.2em</p>
     ```
     
- **Word-Spacing**📎  
  Untuk mengatur jarak antar kata dalam teks.  
  Dengan ini, kamu bisa membuat teks terlihat lebih renggang atau lebih rapat, sesuai kebutuhan tipografi atau desain.  
  Value `word-spacing` ada 3 yaitu:  

  1. **normal**  
     ```html
     <p style="word-spacing: normal;">Teks dengan jarak kata normal</p>
     ```

  2. **px (pixel)**  
     ```html
     <p style="word-spacing: 10px;">Teks dengan jarak kata 10px</p>
     ```

  3. **em (relative unit)**  
     ```html
     <p style="word-spacing: 0.5em;">Teks dengan jarak kata 0.5em</p>
     ```
     
